# mysqlTableMd
mysqldumpコマンドで出力したXMLをxslでいい感じに整形する

mysqldump --no-data --xml exsampleDBSchema -p -h localhost -P 3308 --protocol=tcp > schema.xml

xsltproc -o outputFile style.xsl schema.xml
