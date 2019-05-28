this index has been generated with the following command:

java -server -Xmx60G -cp /home/khast/terrier-core-4.2/etc/:/home/khast/terrier-core-4.2/target/terrier-core-4.2-jar-with-dependencies.jar \
	-Dterrier.etc=/home/khast/terrier-core-4.2/etc \
	-Dterrier.setup=/home/khast/terrier-core-4.2/etc/terrier.properties \
	-Dterrier.index.path=/data/khast/index-java/cw09b_full \
	-Dterrier.index.prefix=cw09b_full \
		org.terrier.applications.TrecTerrier -i -j

and the local terrier.properties file.

To index with Terrier 5, please git clone terrier-core:

    git clone https://github.com/terrier-org/terrier-core

create symbolic links to terrier.properties and collection09.spec in the etc folder, and run:

    export TERRIER_HEAP_MEM=40G
    export TERRIER_OPTIONS="-Dterrier.index.path=/data/khast/index-java/t5/cw09b -Dterrier.index.prefix=cw09b.nostem.nostop"
    ./bin/terrier batchindexing -j -p
