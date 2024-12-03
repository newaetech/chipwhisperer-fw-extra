This repostiory contains firmware files required to build firmware for targets not included in ChipWhisperer Start Kits. This repository isn't meant to be used standalone. Instead, you should use `git submodule`
on the main ChipWhisperer repo:

```bash
cd chipwhisperer/firmware/mcu/hal
git submodule update --init chipwhisperer-fw-extra

# Build firmware example
cd ../simpleserial-base
make PLATFORM=CW308_K82F CRYPTO_TARGET=NONE
```
