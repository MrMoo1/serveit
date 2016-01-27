A really simple HTTP server, written in python, designed for transferring a few files on a local network.

## Installing ##
```
wget http://serveit.googlecode.com/files/serveit-0.1.tar.gz
tar xzf serveit-0.1.tar.gz
cd serveit-0.1
sudo python setup.py install
```

## Usage ##
For example, to serve the file `file.txt` and the directory `dir` on port `8080`:
```
serveit -p 8080 file.txt dir/
```
The port defaults to 80 if the -p option is not included.
To access these files, enter `http://[address]:8080/` into a web browser on another computer on the same network, where `[address]` is the address or host name of the computer that serveit is running on.