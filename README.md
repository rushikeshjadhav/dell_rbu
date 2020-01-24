# dell_rbu

## To build the driver yourself, go on your docker host and use follwing shell commands to build it.

mkdir driver-dell_rbu

cd driver-dell_rbu

git clone https://github.com/xcp-ng/xcp-ng-build-env

git clone https://github.com/rushikeshjadhav/dell_rbu.git

chown 1000 ./dell_rbu/ -R

./xcp-ng-build-env/run.py -b 7.6 --build-local dell_rbu/ --rm
