# POCO_arm-linux-gnueabihf
Cross compile C++ Network Library __POCO__  
__Requirement:__  
openssl-1.1.0  
## Download File
```bash
wget https://pocoproject.org/releases/poco-1.9.0/poco-1.9.0.tar.gz
tar xvf poco-1.9.0.tar.gz
cd poco-1.9.0
```
## Compile
modify <code>build/config/ARM-Linux</code>
```bash
TOOL = arm-linux-gnueabihf
```
```bash
./configure  --config=ARM-Linux --prefix=/usr/local/poco-arm --no-tests --static --shared
make
sudo make install
```

```bash
./configure --config=ARM-Linux --prefix=/usr/local/poco-arm-10 --no-samples --no-tests --everything --static --shared --odbc-lib=/usr/local/unixodbc-arm/lib --odbc-include=/usr/local/unixodbc-arm/include
```
