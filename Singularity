Bootstrap: docker
From: centos:7

%post
    echo "Updating..."
    yum clean all; yum -y update

    echo "Installing CentOS IB stack..."
    yum -y install dapl dapl-utils ibacm infiniband-diags libibverbs libibverbs-devel libibverbs-utils libmlx4 librdmacm librdmacm-utils mstflint opensm-libs perftest qperf rdma

    echo "Creating mount points..."
    mkdir -p /scratch/local
    mkdir -p /software
