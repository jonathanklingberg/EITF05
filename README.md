EITF05
======

Webshop
======
/Users/Jonathan/sites/platslageri/wordpress
	Rootpass: 'rootpass';
	CREATE USER 'webuser' IDENTIFIED BY 't0ps3cr3tp4ssw0rd';
	GRANT SELECT, INSERT, UPDATE, DELETE ON webshop.* TO 'webuser'@'localhost';
	CREATE  TABLE `webshop`.`members` (
  	`username` VARCHAR(22) NOT NULL ,
  	`password_hash` VARCHAR(13) NOT NULL ,
  	`salt` VARCHAR(22) NOT NULL ,
  	`address` VARCHAR(45) NOT NULL ,
  	`member_since` DATETIME NOT NULL ,
  	`last_pw_modify_date` DATETIME NOT NULL ,
  	PRIMARY KEY (`username`) );
SSL:
http://tommcfarlin.com/enable-ssl-in-mamp/

tail -f /Applications/MAMP/logs/php_error.log 
