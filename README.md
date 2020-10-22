# Updated fork of iPXE that is compatible with xNBA/xCAT

Usage:
Build this like a normal iPXE binary (see also https://ipxe.org/download):
```
git checkout v1.20.1-xnba
make bin-x86_64-efi/ipxe.efi
```
Then copy the resulting binary to `/tftpboot/xcat/`:
```
mv bin-x86_64-efi/ipxe.efi /tftpboot/xcat/xnba_1.20.1.efi
cd /tftpboot/xcat
chmod 644 xnba_1.20.1.efi

mv xnba.efi xnba_1.0.3.efi
ln -s xnba_1.20.1.efi xnba.efi

```

