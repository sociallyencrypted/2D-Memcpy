# 2D-Memcpy
A patch to the linux kernel to add a syscall to do a memcpy on a 2D Array. Made for the course CSE231: Operating Systems

## Apply
```bash
gh repo clone torvalds/linux
gh repo clone sociallyencrypted/2D-Memcpy
cp 2D-Memcpy/patchfile.patch linux/patchfile.patch
cd linux
git am patchfile.patch
make menuconfig
make -j $(nproc) && make modules_install && make install
```
