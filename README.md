# iptv-web-sniff
A web stream sniff and proxy tool

## dependencies
This tool only support python3 and requires m3u8 package.
```console
$ pip3 install -U m3u8
```

## usage

### sniff web stream
```console
$ python3 iptv-sniff.py -c tvdb.txt -o playlist/
```
This will sniff all the APIs listed in tvdb.txt and dump a m3u playlist named webtv.m3u,
then please use iptv player to add webtv.m3u when finished.

And enjoy it!

### iptv proxy server
```console
$ python3 iptv-proxy.py -c tvdb.txt&
```
make your own m3u playlist with proxy stream:

Example:
http://192.168.1.1:8080/channel?cnn.m3u8
