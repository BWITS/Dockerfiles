FROM centos:centos6
MAINTAINER Bill W
RUN rpm -ivh http://yum.puppetlabs.com/puppetlabs-release-el-6.noarch.rpm
RUN yum -y update
RUN yum -y install puppet hiera facter
RUN puppet resource package puppet ensure=latest
RUN puppet resource package facter ensure=latest
RUN puppet resource package hiera  ensure=latest
