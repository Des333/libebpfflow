FROM debian:sid

RUN apt-get update -y

#RUN apt-get install -y git procps linux-headers-$(uname -r)
RUN apt-get install -y git procps linux-headers-5.4.0-3-amd64

# Requirements from libebpfflow README
RUN apt-get install -y \
  build-essential \
  autoconf \
  automake \
  autogen \
  libjson-c-dev \
  pkg-config \
  libzmq3-dev \
  libcurl4-openssl-dev \
  libbpfcc-dev

RUN git clone https://github.com/ntop/libebpfflow && cd /libebpfflow && ./autogen.sh && make

CMD ["/libebpfflow/ebpflowexport", "-tuio"]
