SpringPasswordEncoder
===
A simple tool to generate spring [BCryptPasswordEncoder](https://docs.spring.io/spring-security/site/docs/current/apidocs/org/springframework/security/crypto/bcrypt/BCryptPasswordEncoder.html) hashes, and also to verify existing hashes. This is just to generate hashes for [Kylin](http://kylin.apache.org/docs/howto/howto_ldap_and_sso.html) where the admin password is unfortunately [hardcorded](https://github.com/KylinOLAP/Kylin/blob/ab0118647200f7704db79e4b2a76e4588616c27d/server/src/main/resources/kylinSecurity.xml), but I guess can be used for other purposes as well.

## Build

$ mvn package

## Usage

```bash
$ java -jar target/spring-password-0.1.0.jar
 -e : Encode password into hash (default: false)
 -v : Verify hash (default: false)
 ```
