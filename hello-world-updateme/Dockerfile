FROM registry.access.redhat.com/rhel7:7.0-21 

RUN yum -y install python-pip; yum clean all

ADD . /src

RUN cd /src; pip install -r requirements.txt

EXPOSE 8080

CMD ["python", "/src/index.py"]
