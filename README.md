# HDInsight-ESP-Kafka-Spark

Use these templates to create HDInsight Kafka and Spark clusters with the Enterprise Security Package (ESP) in peered VNETs. This assumes you have already set up Azure Active Directory Domain Services (AADDS) and have a managed identity (MI).

## template_vnet.json

Use this template to create a VNET and peer it to the VNET that contains your Azure Active Directory Domain Services. This should be used twice to create a VNET for each of the 2 HDInisght clusters (Kafka and Spark)

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Ftylerfox%2FHDInsight-ESP-Kafka-Spark%2Fmaster%2Ftemplate_vnet.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Ftylerfox%2FHDInsight-ESP-Kafka-Spark%2Fmaster%2Ftemplate_vnet.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

## template_peer.json

Once you have created the 2 VNETs, use this template to peer them to each other.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Ftylerfox%2FHDInsight-ESP-Kafka-Spark%2Fmaster%2Ftemplate_peer.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Ftylerfox%2FHDInsight-ESP-Kafka-Spark%2Fmaster%2Ftemplate_peer.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

## template_kafka.json

Once the two VNETs are set up and peered, use this template to deploy an HDInsight Kafka cluster in one of the VNETs.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Ftylerfox%2FHDInsight-ESP-Kafka-Spark%2Fmaster%2Ftemplate_kafka.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Ftylerfox%2FHDInsight-ESP-Kafka-Spark%2Fmaster%2Ftemplate_kafka.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

## template_spark.json

Finally, use this template to deploy an HDInsight Spark cluster in the other VNET.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Ftylerfox%2FHDInsight-ESP-Kafka-Spark%2Fmaster%2Ftemplate_spark.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Ftylerfox%2FHDInsight-ESP-Kafka-Spark%2Fmaster%2Ftemplate_spark.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>