FROM centos:centos7

RUN yum install -y -q https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm && \
    yum install -y -q gcc-c++ tbb-devel libX11-devel libXt-devel net-tools wget which openssl-devel git && \
    yum clean -y -q all

RUN wget -q https://files.salome-platform.org/Salome/Salome9.5.0/SALOME-9.5.0-CO7-SRC.tar.gz && \
    tar -zxvf SALOME-9.5.0-CO7-SRC.tar.gz -C /tmp SALOME-9.5.0-CO7-SRC/BINARIES-CO7 SALOME-9.5.0-CO7-SRC/ARCHIVES && \
    mkdir /tmp/INSTALL && \
    mkdir /tmp/ARCHIVES && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/CAS /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/cgns /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/cmake /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/cppunit /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/doxygen /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/eigen /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/embree /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/FIELDS /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/freeimage /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/freetype /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/GEOM /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/gmsh /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/graphviz /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/GUI /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/hdf5 /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/homard_bin /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/ispc /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/KERNEL /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/lapack /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/LIBBATCH /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/libxml2 /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/llvm /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/matplotlib /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/MEDCOUPLING /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/medfile /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/mesa /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/MeshGems /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/metis /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/netgen /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/nlopt /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/omniORB /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/omniORBpy /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/opencv /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/ospray /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/ParaView /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/PARAVIS /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/planegcs /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/PyQt /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/pyreadline /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/Python /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/qt /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/qwt /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/SALOME /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/scotch /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/SHAPER /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/SHAPERSTUDY /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/sip /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/SMESH /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/swig /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/tcl /tmp/INSTALL/ && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/BINARIES-CO7/tk /tmp/INSTALL/ && \
    rm -rf /tmp/INSTALL/Python/lib/python3.6/site-packages/numpy* && \
    mv /tmp/SALOME-9.5.0-CO7-SRC/ARCHIVES/CONFIGURATION.tgz /tmp/ARCHIVES && \
    rm -rf SALOME-9.5.0-CO7-SRC.tar.gz /tmp/SALOME-9.5.0-CO7-SRC 