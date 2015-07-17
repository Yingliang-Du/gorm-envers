# gorm-envers
A Grails Plugin for GORM domain audit using Hibernate Envers

## Install this project
```
git clone https://github.com/Yingliang-Du/gorm-envers.git
cd gorm-envers
grails clean
grails compile
grails install
```
Start audit Domain classes in your Grails application:

Add plugin dependency
```
compile ("org.grails.plugins:gorm-envers:0.1-SNAPSHOT") {
	exclude module: 'hibernate-core'
	exclude module: 'hibernate-entitymanager'
}
```

Add @Audited annotation to the domain class you want to audit

That is it!
