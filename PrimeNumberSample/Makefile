all: build

app.keystore:
	echo y | keytool -genkeypair -dname "cn=sample, ou=sample, o=sample, c=sample" -alias applinkprimenumber -keypass android -keystore ./app.keystore -storepass android -validity 10000

build: app.keystore
	gradle --no-daemon -q build

.PHONY: build
