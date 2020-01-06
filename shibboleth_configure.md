
For most of the configuration part I followed this tutorial: http://federation.belnet.be/files/idp_shibboleth_v3_linux.pdf

```
had to add http://repo1.maven.org/maven2/javax/servlet/jstl/1.2/jstl-1.2.jar and http://repo1.maven.org/maven2/javax/servlet/jsp-api/2.0/jsp-api-2.0.jar
in WEB-INF
/opt/shibboleth-idp/edit-webapp/WEB-INF/lib/
```

```
export IDP_VERSION="3.4.4"
export SHIB_HOME=/opt/shibboleth-idp
export SHIB_INST_HOME=/root/shibboleth-identity-provider-$IDP_VERSION
export IDP_HOME=/opt/shibboleth-idp
export JAVA_HOME=/usr
```

```
apt-get install libjstl1.1-java
a2enmod ssl
a2enmod proxy_http
a2enmod proxy_ajp
```