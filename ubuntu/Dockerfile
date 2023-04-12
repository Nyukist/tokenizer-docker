FROM ubuntu

RUN apt-get update
RUN apt-get install -y vim
# RUN useradd python-useradd
# RUN mkdir /home/python-user

RUN apt-get upgrade -y python3
RUN apt-get install -y python3-tk
RUN apt-get install -y python3-venv
RUN apt-get install -y python3-pip
RUN apt-get install -y git
RUN apt-get install -y default-jdk
RUN apt-get install -y iputils-ping

# RUN mkdir ./work

WORKDIR /home/python-user/work
RUN cd /home/python-user/work
RUN git clone https://github.com/Nyukist/tokenizer.git
RUN cd /home/python-user/work/tokenizer
RUN python3 -m venv .venv
RUN pip install peewee
CMD ["tail", "-f", "/dev/null"]

