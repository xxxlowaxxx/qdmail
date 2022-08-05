Qdmail
======

Qdmail library series.  
Test has been run on PHP 5.2, 5.3, 5.4, 5.5, 5.6.

[![Build Status](https://travis-ci.org/ftngrn/qdmail.png?tag=php-5)](https://travis-ci.org/ftngrn/qdmail)

This series forked from http://hal456.net/

* [Qdmail](http://hal456.net/qdmail/)
* [QdmailReceiver](http://hal456.net/qdmail_rec/)
* [Qdsmtp](http://hal456.net/qdsmtp/)

## このライブラリについて ##
Qdmailライブラリシリーズのgithub版です。  
開発者のspokさんから以下のように許可を頂いています。  
```
ライセンスに従って頂ければ何をしていただいても構いません。
多くの人に使われることが私の幸せです。
ただ、本業が忙しく、qdmailを触る時間は、もうとれないだろうと思っております。
できれば私の手を離れて誰かが管理してくれるとうれしいと思っています。
```

## Receiver ##
Azure ADのサービスプリンシパルを利用したOAuth2.0認証によるPOP接続を追加  
証明書を使う方式です。テストしていないので使用は自己責任でお願いします。  
qdmail_receiver.phpの以下の箇所に、環境に応じた値を入力します。  
```
var $server = array(
		'host'=>'',
		'port'=>110,
		'user'=>'',
		'pass'=>'',
	);

	var $certificate = array(
		'path'=>'', //pfx file only
		'pwd' =>''
	);

	var $service_principal = array(
		'client_id'=>'',
		'tenant_id'=>''
	);

	var $auth = 'BASIC'; // or XOAUTH2
```

## Associated repository ##
* [Component for CakePHP2.x](https://github.com/spark-lab/Qdmail) by spark-lab

## License ##

The MIT License (MIT)

## Copyright ##

Qdmail  
Copyright (C)2008    spok  
http://hal456.net/qdmail_rec/  
http://www.cpa-lab.com/tech/  
