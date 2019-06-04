Bootstrap: docker
From: debian:stretch-slim

%labels
Author "Randall Cab White - rcwhite@stanford.edu"


#########
#%setup
#########

#Downlaod packages
%post
  apt-get -ym update
  apt-get -ym install wget firefox-esr bzip2
	wget -O firefox.tar.bz2 "https://download.mozilla.org/?product=firefox-devedition-latest-ssl&os=linux64&lang=en-US"
	tar xvf firefox.tar.bz2
%environment
  export IMAGE_NAME="firefox_dev_edition"
%runscript
	/firefox/firefox-bin
