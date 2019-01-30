this index has been generated with the following command on node1.novello.isti.cnr.it:

java -server -Xmx30G -cp /home/khast/terrier-core/etc/:/home/khast/terrier-core/target/terrier-core-4.2-jar-with-dependencies.jar \
	-Dterrier.etc=/home/khast/terrier-core/etc \
	-Dterrier.setup=/home/khast/terrier-core/etc/terrier.properties \
	-Dterrier.index.path=/data/khast/index-java/cw12b_full \
	-Dterrier.index.prefix=cw12b_full \
		org.terrier.applications.TrecTerrier -i -j

and the local terrier.properties file.
