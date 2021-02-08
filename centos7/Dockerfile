FROM centos:centos7

RUN yum install -y -q https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm && \
    yum install -y -q gcc-c++ gcc-gfortran python3 make tbb-devel libX11-devel libXt-devel net-tools wget which openssl-devel git libicu && \
    yum clean -y -q all && python3 -m pip install numpy openpyxl

RUN wget -q https://files.salome-platform.org/Salome/Salome9.5.0/SALOME-9.5.0-CO7-SRC.tar.gz && \
    tar -zxvf SALOME-9.5.0-CO7-SRC.tar.gz -C /tmp SALOME-9.5.0-CO7-SRC/BINARIES-CO7 SALOME-9.5.0-CO7-SRC/ARCHIVES && \
    mkdir /tmp/INSTALL && \
    mkdir /tmp/ARCHIVES && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/* /tmp/INSTALL/ && \
    rm -rf /tmp/INSTALL/Python/lib/python3.6/site-packages/numpy* && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/ARCHIVES/CONFIGURATION.tgz /tmp/ARCHIVES && \
    rm -rf SALOME-9.5.0-CO7-SRC.tar.gz /tmp/SALOME-9.5.0-CO7-SRC 
