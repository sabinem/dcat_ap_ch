# DCAT-AP-CH

This github repo is intended to prepare the further development of 
DCAT-AP-CH by providing a definition area for all its documents.

## About

The Specification uses respec: https://respec.org/docs/

## Deploy to a Static Server

Staging is running at:

```
https://dcat-ap-ch-def.clients.liip.ch/
```

Get to server:

```
ssh -p 2202 -l liip ps8.ms.bsa.oriented.ch
cd /var/www/html/dcat-ap-ch-def.clients.liip.ch/
```

deploy documents

```
tar -zcf dcat-ap-ch-def.tar.gz docs/
scp -P 2202 dcat-ap-ch-def.tar.gz liip@ps8.ms.bsa.oriented.ch:/var/www/html/dcat-ap-ch-def.clients.liip.ch/
ssh -p 2202 -l liip ps8.ms.bsa.oriented.ch
cd /var/www/html/dcat-ap-ch-def.clients.liip.ch
tar -xzf dcat-ap-ch-def.tar.gz
cd docs
mv * ..
rmdir docs
``` 

Now the site should be reachable at https://ogdch-new-convention-handbook.clients.liip.ch.



