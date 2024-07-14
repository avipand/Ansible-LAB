# Use the official Ubuntu base image
FROM ubuntu:latest

# Install necessary packages
RUN apt-get update && \
    apt-get install -y software-properties-common sudo \
    && add-apt-repository --yes --update ppa:ansible/ansible  \
    && apt-get install -y ansible \
    && apt-get install -y iputils-ping \
    && apt-get install -y openssh-server  \
    && service ssh start \
    && apt-get clean

# Create ansible user with password 'ansible'
RUN useradd -m ansible && echo "ansible:ansible" | chpasswd

# Give ansible user sudo privileges
RUN usermod -aG sudo ansible

# Allow ansible user to execute sudo commands without a password
RUN echo "ansible ALL=(ALL) NOPASSWD: ALL" >> /etc/sudoers

# Set environment variables
ENV ANSIBLE_HOME /home/ansible

# Switch to ansible user
USER ansible

# Set working directory
WORKDIR $ANSIBLE_HOME

# Expose port 22 (for SSH, if necessary)
EXPOSE 22
