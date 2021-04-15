# EigenCC: Confidential Computation

## Intel SGX

[Intel SGX](https://software.intel.com/content/www/us/en/develop/topics/software-guard-extensions.html) Enhance Your Code and Data Protection

### Compile

```
$ cd cc/sgx 
$ docker run --name fns --net=host -v$(pwd):/app -w /app -it teaclave/teaclave-build-ubuntu-1804-sgx-2.9.1 bash
# mkdir -p build && cd build
# cmake -DTEST_MODE=ON .. && make
```

### Run
```
# cd /teaclave/release/services
# export IAS_SPID=xxxx
# export IAS_KEY=xxx
# ./fns
```

## ARM TrustZone on FPGA 
