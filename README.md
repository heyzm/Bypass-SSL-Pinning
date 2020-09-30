# Bypass-SSL-Pinning

## 使用教程

1. 推送burp证书到设备上

```shell
$ adb push burpca-cert-der.crt /data/local/tmp/cert-der.crt
```

2. 启动frida

```shell
$ frida -U -f it.app.mobile -l frida-android-repinning.js --no-pause
```

## 参考资料:

1. https://techblog.mediaservice.net/2017/07/universal-android-ssl-pinning-bypass-with-frida/%
