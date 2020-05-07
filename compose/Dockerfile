#ARG PYTHON_VERSION="3.8"
FROM alpine

RUN apk update; \
    apk upgrade;

RUN apk add tzdata
RUN ln -s /usr/share/zoneinfo/Pacific/Honolulu /etc/localtime
RUN echo "Pacific/Honolulu" >  /etc/timezone

RUN apk add imagemagick vlc libjpeg-turbo-utils
RUN apk add xauth
RUN apk add firefox-esr curl wget
RUN apk add busybox-extras
	
RUN apk add alpine-sdk gfortran automake libtool autoconf
RUN apk add freetype-dev jpeg-dev
RUN apk add libxml2-dev
RUN apk add xmlsec-dev
RUN ln -s /usr/include/libxml2/libxml /usr/include/libxml

RUN apk add python3 python3-dev
RUN apk add py3-pip python3-tkinter

RUN pip3 install --upgrade pip
RUN pip3 install cython
RUN pip3 install numpy
RUN pip3 install matplotlib
RUN pip3 install pandas
RUN pip3 install astropy
RUN pip3 install ephem
RUN pip3 install Pillow
RUN pip3 install bs4
RUN pip3 install lxml
RUN pip3 install Pygments

CMD tail -f /dev/null
