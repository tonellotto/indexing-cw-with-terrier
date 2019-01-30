this index has been generated with the following command:

java -server -Xmx60G -cp /home/khast/terrier-core-4.2/etc/:/home/khast/terrier-core-4.2/target/terrier-core-4.2-jar-with-dependencies.jar \
	-Dterrier.etc=/home/khast/terrier-core-4.2/etc \
	-Dterrier.setup=/home/khast/terrier-core-4.2/etc/terrier.properties \
	-Dterrier.index.path=/data/khast/index-java/cw09b_full \
	-Dterrier.index.prefix=cw09b_full \
		org.terrier.applications.TrecTerrier -i -j

and the local terrier.properties file.
