![image](images/confluent-logo-300-2.png)

# About

Template configurations for Apache Kafka® clients and Confluent Platform components


# How to use these template files

1. Determine which of the files you need:

   * [Java client to Confluent Cloud](java.config)
   * [Java client to Confluent Cloud with Confluent Cloud Schema Registry](java-sr.config)
   * [librdkafka-based client to Confluent Cloud](librdkafka.config)
   * [librdkafka-based client to Confluent Cloud with Confluent Cloud Schema Registry](librdkafka-sr.config)

2. Copy the file locally.

3. Customize the file with connection information to your Kafka cluster. Notice that the file cannot be used as-is because it has parameters that need to be substituted with real values.

   * If you are connecting to [Confluent Cloud](https://www.confluent.io/confluent-cloud/?utm_source=github&utm_medium=demo&utm_campaign=ch.examples_type.community_content.clients-ccloud), you need to provide the bootstrap servers and API key and secret: here is how to create or find [those values](https://docs.confluent.io/current/cloud/using/config-client.html#librdkafka-based-c-clients?utm_source=github&utm_medium=demo&utm_campaign=ch.examples_type.community_content.clients-ccloud).

5. (optional) If you are using a librdkafka-based client, additional configuration properties are supported. See [CONFIGURATION.md](https://github.com/edenhill/librdkafka/blob/master/CONFIGURATION.md) for the full list.		
