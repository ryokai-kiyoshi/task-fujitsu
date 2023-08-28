
```
[accope@AP-SA01 ssoam]$ cat setup.info 
Setup Date:2021/10/22 06:59:31
[accope@AP-SA01 ssoam]$ 

```


```
[accope@AP-SA01 ssoam]$ more setup_ssoam.log 
/opt/syncdot/auth/ssoam/setup/./lib/ssoam_setup_tomcat.sh service-install syncdot-auth-ssoam
Created symlink /etc/systemd/system/multi-user.target.wants/syncdot-auth-ssoam.service → /usr/lib/systemd/system/syncdot-auth-ssoam.service.
/opt/syncdot/auth/ssoam/setup/./lib/ssoam_setup_permission.sh tomcat_syncdot /opt/syncdot/auth/tomcat/ssoam syncdot syncdot-auth-ssoam
/opt/syncdot/auth/ssoam/setup/./lib/ssoam_setup_tomcat.sh service-start syncdot-auth-ssoam
ssoam: INFO: ssoam31009: Tomcatサービスの起動に成功しました。Name=syncdot-auth-ssoam
ssoam: INFO: ssoam31001: Tomcatのセットアップが正常に終了しました。
/opt/syncdot/auth/ssoam/setup/./lib/ssoam_setup_openam.sh /opt/syncdot/auth/ssoam/.openam_configuration.properties /var/syncdot/auth syncdot
java.net.ConnectException: Connection refused (Connection refused)
	at java.net.PlainSocketImpl.socketConnect(Native Method)
	at java.net.AbstractPlainSocketImpl.doConnect(AbstractPlainSocketImpl.java:350)
	at java.net.AbstractPlainSocketImpl.connectToAddress(AbstractPlainSocketImpl.java:206)
	at java.net.AbstractPlainSocketImpl.connect(AbstractPlainSocketImpl.java:188)
	at java.net.SocksSocketImpl.connect(SocksSocketImpl.java:392)
	at java.net.Socket.connect(Socket.java:607)
	at java.net.Socket.connect(Socket.java:556)
	at sun.net.NetworkClient.doConnect(NetworkClient.java:180)
	at sun.net.www.http.HttpClient.openServer(HttpClient.java:463)
	at sun.net.www.http.HttpClient.openServer(HttpClient.java:558)
	at sun.net.www.http.HttpClient.<init>(HttpClient.java:242)
	at sun.net.www.http.HttpClient.New(HttpClient.java:339)
	at sun.net.www.http.HttpClient.New(HttpClient.java:357)
	at sun.net.www.protocol.http.HttpURLConnection.getNewHttpClient(HttpURLConnection.java:1226)
	at sun.net.www.protocol.http.HttpURLConnection.plainConnect0(HttpURLConnection.java:1162)
	at sun.net.www.protocol.http.HttpURLConnection.plainConnect(HttpURLConnection.java:1056)
	at sun.net.www.protocol.http.HttpURLConnection.connect(HttpURLConnection.java:990)
	at com.sun.identity.setup.OpenSSOConfigurator.postRequestToServer(OpenSSOConfigurator.java:246)
	at com.sun.identity.setup.OpenSSOConfigurator.execute(OpenSSOConfigurator.java:142)
	at com.sun.identity.setup.Main.main(Main.java:32)
java.net.ConnectException: Connection refused (Connection refused)
	at java.net.PlainSocketImpl.socketConnect(Native Method)
	at java.net.AbstractPlainSocketImpl.doConnect(AbstractPlainSocketImpl.java:350)
	at java.net.AbstractPlainSocketImpl.connectToAddress(AbstractPlainSocketImpl.java:206)
	at java.net.AbstractPlainSocketImpl.connect(AbstractPlainSocketImpl.java:188)
	at java.net.SocksSocketImpl.connect(SocksSocketImpl.java:392)
	at java.net.Socket.connect(Socket.java:607)
	at java.net.Socket.connect(Socket.java:556)
	at sun.net.NetworkClient.doConnect(NetworkClient.java:180)
	at sun.net.www.http.HttpClient.openServer(HttpClient.java:463)
	at sun.net.www.http.HttpClient.openServer(HttpClient.java:558)
	at sun.net.www.http.HttpClient.<init>(HttpClient.java:242)
	at sun.net.www.http.HttpClient.New(HttpClient.java:339)
	at sun.net.www.http.HttpClient.New(HttpClient.java:357)
	at sun.net.www.protocol.http.HttpURLConnection.getNewHttpClient(HttpURLConnection.java:1226)
	at sun.net.www.protocol.http.HttpURLConnection.plainConnect0(HttpURLConnection.java:1162)
	at sun.net.www.protocol.http.HttpURLConnection.plainConnect(HttpURLConnection.java:1056)
	at sun.net.www.protocol.http.HttpURLConnection.connect(HttpURLConnection.java:990)
	at org.forgerock.openam.installer.utils.StatusChecker.run(StatusChecker.java:69)
	at java.lang.Thread.run(Thread.java:748)
コマンドの実行に失敗しました。Command=/opt/syncdot/auth/ssoam/setup/./lib/ssoam_setup_openam.sh Result=255
/opt/syncdot/auth/ssoam/setup/./lib/ssoam_setup_openam.sh /opt/syncdot/auth/ssoam/.openam_configuration.properties /var/syncdot/auth syncdot
null
Configuration Failed.  The server returned error code :500
コマンドの実行に失敗しました。Command=/opt/syncdot/auth/ssoam/setup/./lib/ssoam_setup_openam.sh Result=255
/opt/syncdot/auth/ssoam/setup/./lib/ssoam_setup_openam.sh /opt/syncdot/auth/ssoam/.openam_configuration.properties /var/syncdot/auth syncdot
Already Configured!
ssoam: INFO: ssoam32001: SSOAMのセットアップが正常に終了しました。
unzip /opt/syncdot/auth/ssoam/setup/auth/media/SSOAdminTools-13.0.0.zip -d /opt/syncdot/auth/ssoam/ssoadmtools
Archive:  /opt/syncdot/auth/ssoam/setup/auth/media/SSOAdminTools-13.0.0.zip
   creating: /opt/syncdot/auth/ssoam/ssoadmtools/template/
   creating: /opt/syncdot/auth/ssoam/ssoadmtools/template/unix/
   creating: /opt/syncdot/auth/ssoam/ssoadmtools/template/unix/bin/
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/template/unix/bin/ssoadm.template  
   creating: /opt/syncdot/auth/ssoam/ssoadmtools/template/windows/
   creating: /opt/syncdot/auth/ssoam/ssoadmtools/template/windows/bin/
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/template/windows/bin/ssoadm.bat.template  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/template/unix/bin/ampassword.template  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/template/windows/bin/ampassword.bat.template  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/template/unix/bin/amverifyarchive.template  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/template/windows/bin/amverifyarchive.bat.template  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/template/unix/bin/verifyarchive.template  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/template/windows/bin/verifyarchive.bat.template  
   creating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/activation-1.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/assertj-core-2.1.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/authz-framework-3.1.5.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/authz-framework-api-3.1.5.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/bsh-2.0b4.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/cc-2008-08-08.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/chf-client-apache-common-3.0.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/chf-client-apache-sync-3.0.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/chf-http-core-3.0.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/chf-http-servlet-3.0.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/click-extras-2.3.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/click-nodeps-2.3.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/commons-codec-1.6.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/commons-collections-3.2.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/commons-fileupload-1.2.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/commons-io-2.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/commons-lang-2.6.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/commons-logging-1.1.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/commons-logging-api-1.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/esapiport-2013-12-04.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/FastInfoset-1.2.13.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-audit-core-4.1.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-audit-handler-csv-4.1.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-audit-handler-jdbc-4.1.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-audit-handler-syslog-4.1.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-audit-json-4.1.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-bloomfilter-core-1.0.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-bloomfilter-monitoring-1.0.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-guava-annotations-18.0.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-guava-base-18.0.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-guava-cache-18.0.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-guava-collect-18.0.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-guava-concurrent-18.0.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-guava-escape-18.0.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-guava-hash-18.0.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-guava-io-18.0.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-guava-math-18.0.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-guava-net-18.0.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-guava-primitives-18.0.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-guice-core-1.1.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-jaspi-jwt-session-module-3.1.5.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-jaspi-runtime-3.1.5.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-persistit-core-4.3.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-selfservice-core-1.0.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-test-utils-3.0.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/forgerock-util-3.0.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/freemarker-2.3.19.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/grizzly-framework-2.3.23.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/grizzly-http-2.3.23.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/grizzly-http-server-2.3.23.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/grizzly-http-servlet-2.3.23.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/groovy-2.3.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/groovy-json-2.3.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/groovy-jsr223-2.3.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/groovy-sandbox-1.6.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/guice-3.0-no_aop.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/guice-assistedinject-3.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/guice-multibindings-3.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/hamcrest-core-1.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/HdrHistogram-2.1.4.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/HikariCP-2.4.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/httpclient-4.4.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/httpcore-4.4.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/i18n-core-1.4.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/i18n-slf4j-1.4.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/isorelax-20030108.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jackson-annotations-2.4.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jackson-core-2.4.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jackson-databind-2.4.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jackson-dataformat-csv-2.6.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jackson-dataformat-smile-2.4.4.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jackson-dataformat-xml-2.4.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jackson-dataformat-yaml-2.4.4.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jackson-module-jaxb-annotations-2.6.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jackson-module-jsonSchema-2.6.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jato-2005-05-04.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/java-ipv6-0.14.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/javax.mail-1.5.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/javax.security.auth.message-3.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/javax.servlet-api-3.0.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jaxb-api-1.0.6.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jaxb-impl-1.0.6.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jaxb-libs-1.0.6.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jaxb-xjc-1.0.6.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jaxb1-impl-2.0.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jaxp-api-1.4.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jaxrpc-api-1.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jaxrpc-impl-1.1.3_01-041406.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jaxrpc-spi-1.1.3_01.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jcommander-1.27.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jdmkrt-2007-01-10.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/je-5.0.104.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jersey-bundle-1.1.1-ea.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jersey-client-1.1.5.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jersey-core-1.1.5.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jgrapht-core-0.9.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/joda-time-2.7.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/json-20090211.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/json-resource-4.0.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/json-resource-http-4.0.3.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/json-web-token-3.0.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jsr305-3.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jsr311-api-1.1.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jss4-2007-08-11.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/jstl-1.1.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/junit-4.10.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/log4j-over-slf4j-1.7.5.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/mail-1.4.5.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/mimepull-1.7.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/mockito-all-1.9.5.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/oauth-client-1.1.5.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/oauth-server-1.1.5.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/oauth-signature-1.1.5.2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/oauth2-core-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/ognl-2.6.9.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-annotations-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-audit-configuration-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-audit-context-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-audit-core-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-auth-scripted-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-certs-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-cli-definitions-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-cli-impl-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-core-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-core-rest-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-coretoken-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-dashboard-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-dtd-schema-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-entitlements-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-federation-library-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-http-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-http-client-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-idpdiscovery-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-idsvcs-schema-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-installtools-launcher-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-jaxrpc-schema-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-ldap-utils-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-liberty-schema-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-license-core-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-license-manager-cli-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-license-servlet-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-mib-schema-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-oauth-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-restlet-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-saml2-schema-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-scripting-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-shared-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-tokens-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-wsfederation-schema-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/openam-xacml3-schema-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/opendj-cli-3.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/opendj-config-3.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/opendj-core-3.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/opendj-grizzly-3.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/opendj-rest2ldap-3.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/opendj-server-3.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/opendj-server-legacy-3.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/OpenFM-13.0.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/org.apache.servicemix.bundles.javax-inject-1_2.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/org.restlet-2.3.12.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/org.restlet.ext.jackson-2.3.12.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/org.restlet.ext.json-2.3.12.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/org.restlet.ext.servlet-2.3.12.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/org.restlet.ext.slf4j-2.3.12.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/org.restlet.ext.xml-2.3.12.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/publicsuffix-1.0.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/relaxngDatatype-20020414.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/rhino-1.7R4.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/saaj-impl-1.3.19.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/serializer-2.7.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/slf4j-api-1.7.5.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/slf4j-nop-1.7.5.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/snakeyaml-1.6.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/stax2-api-3.1.4.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/super-csv-2.4.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/testng-6.8.5.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/tools-1.7.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/validation-api-1.1.0.Final.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/velocity-1.7.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/woodstox-core-asl-4.3.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/xalan-2.7.1.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/xercesImpl-2.11.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/xml-apis-2.11.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/xml-resolver-2.11.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/xml-serializer-2.11.0.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/xmlsec-1.5.6.jar  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/lib/xsdlib-20060615.jar  
   creating: /opt/syncdot/auth/ssoam/ssoadmtools/legal-notices/
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/legal-notices/license.txt  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/README.setup  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/setup  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/setup.bat  
   creating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/serviceDefaultValues.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/AGBits.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthBasic.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthBasicAuth.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthBasic_en.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthBasic_ja.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthCommonCheck.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthCommonCheckAuth.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthCommonCheck_en.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthCommonCheck_ja.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthCountUp.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthCountUpAuth.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthCountUp_en.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthCountUp_ja.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthGracePeriod.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthGracePeriodAuth.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthGracePeriod_en.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthGracePeriod_ja.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthOptionCheck.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthOptionCheckAuth.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthOptionCheck_en.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthOptionCheck_ja.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthPasswordCheck.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthPasswordCheckAuth.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthPasswordCheck_en.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amAuthPasswordCheck_ja.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/click-page.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/CustomAuthenticationErrorMassage.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/fedletBits.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/fedletJarExtract.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/fmConfiguratorPlugins.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/fmConfiguratorTagSwap.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/fmServiceDefaultValues.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/fmServiceNames.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/webServiceClientUI.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/webServiceProviderUI.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/webServiceSTSUI.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/webServiceUI.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/bootstrap.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/bootstrapConfig.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/configuratorPlugins.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/configuratorTagSwap.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/debugconfig.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/famServiceNames.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/hiddenserverconfig.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/log4j.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/rsa_api.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/schemaNames.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/serviceNames.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/validserverconfig.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/amadm.properties  
  inflating: /opt/syncdot/auth/ssoam/ssoadmtools/resources/agentlocaleprop.properties  
/opt/syncdot/auth/ssoam/ssoadmtools/setup --acceptLicense --path /var/syncdot/auth/ssoam --debug /var/syncdot/log/auth/ssoam/ssoadmtools/debug --
log /var/syncdot/log/auth/ssoam/ssoadmtools/log
/var/syncdot/auth/ssoam/bootstrap (No such file or directory)
コマンドの実行に失敗しました。Command=/opt/syncdot/auth/ssoam/ssoadmtools/setup Result=1
ssoam: ERROR: ssoam33002: Administration Toolsのセットアップに失敗しました。Detail=(/opt/syncdot/auth/ssoam/ssoadmtools/setup)
com.fujitsu.fjh.auth.ssoam.setup.SetupSSOAMException: ssoam: ERROR: ssoam33002: Administration Toolsのセットアップに失敗しました。Detail=(/opt/sy
ncdot/auth/ssoam/ssoadmtools/setup)
	at com.fujitsu.fjh.auth.ssoam.setup.component.ssoam.SetupOpenAMTools.setupOpenAMTools(SetupOpenAMTools.java:106)
	at com.fujitsu.fjh.auth.ssoam.setup.component.ssoam.SetupOpenAMTools.setup(SetupOpenAMTools.java:35)
	at com.fujitsu.fjh.auth.ssoam.setup.cli.SetupCommanderBase.setup(SetupCommanderBase.java:16)
	at com.fujitsu.fjh.auth.ssoam.setup.cli.ssoam.SetupCommander.setup(SetupCommander.java:96)
	at com.fujitsu.fjh.auth.ssoam.setup.cli.ssoam.SetupCommand.setupProcess(SetupCommand.java:155)
	at com.fujitsu.fjh.auth.ssoam.setup.cli.ssoam.SetupCommand.main(SetupCommand.java:51)
ssoam: ERROR: ssoam30002: setup_ssoamコマンドが実行に失敗しました。
```