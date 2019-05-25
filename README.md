![CuseyHub](https://github.com/cusey/ImageForWiki/blob/master/Logos/CuseyHub_Banner_Small.jpg)

# Apache Kafka

<img 
src="https://github.com/cusey/ImageForWiki/blob/master/Logos/ApacheKafka.PNG" 
alt="Apache Kafka" 
height="150px"/>  

## Starting Kafka    
1. Must have install JDK 1.8. Kafka will not work with any other version of the JDK.

2. Download the Kafka zip file at [kafka_2.12-2.2.0.tgz ](https://www.apache.org/dyn/closer.cgi?path=/kafka/2.2.0/kafka_2.12-2.2.0.tgz)

3. Unzip the file to C:\kafka_2.12-2.2.0

4. Add C:\kafka_2.12-2.2.0\bin\windows to the environmental variables

5. Create two folders C:\kafka_2.12-2.2.0\data\zookeeper and C:\kafka_2.12-2.2.0\data\kafka

6. Change the following line code in C:\kafka_2.12-2.2.0\config\zookeeper.properties file. You have to change the bachslash to forwardslash in the windows path. 

```
dataDir=C:/kafka_2.12-2.2.0/data/zookeeper
```
7. Open Windows Command Line type the following commands. Must change directory to kafka folder.

```
C:\Windows\System32>cd C:\kafka_2.12-2.2.0

C:\kafka_2.12-2.2.0>zookeeper-server-start.bat config\zookeeper.properties
```

8. Change the following line code in C:\kafka_2.12-2.2.0\config\server.properties file. You have to change the bachslash to forwardslash in the windows path.

```
dataDir=C:/kafka_2.12-2.2.0/data/kafka
```

9. Open new command line window and enter in the following commands.

```
C:\Windows\System32>cd C:\kafka_2.12-2.2.0

C:\kafka_2.12-2.2.0>kafka-server-start.bat config\server.properties
```

## Authors
* John Cusey - CuseyHub  

## License   
This project is licensed under the MIT License
