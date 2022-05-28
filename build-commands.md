# Build Commands
```sh
git clone https://github.com/galoget/fcrackzip
cd fcrackzip/fcrackzip-1.0
./configure
make
make check
make install
```

# Testing BoF
```sh
┌──(galoget㉿hackem)-[~/fcrackzip/fcrackzip-1.0]
└─$ chmod +x fcrackzip

┌──(galoget㉿hackem)-[~/fcrackzip/fcrackzip-1.0]
└─$ chmod +x fcrackzip

┌──(galoget㉿hackem)-[~/fcrackzip/fcrackzip-1.0]
└─$ ./fcrackzip -p $(python3 -c 'print("A"*40)') file.zip
skipping 'file.zip': No such file or directory
no usable files found

┌──(galoget㉿hackem)-[~/fcrackzip/fcrackzip-1.0]
└─$ ./fcrackzip -p $(python3 -c 'print("A"*180)') file.zip
zsh: segmentation fault  ./fcrackzip -p $(python3 -c 'print("A"*180)') file.zip
```
