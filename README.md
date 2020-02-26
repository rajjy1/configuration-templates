![image](images/confluent-logo-300-2.png)

# About

Template configurations for Apache Kafka® clients and Confluent Platform components


# How to use these template files for Confluent Cloud

These instructions are for users who are looking for template files with clients configurations for [Confluent Cloud](https://www.confluent.io/confluent-cloud/?utm_source=github&utm_medium=demo&utm_campaign=ch.examples_type.community_content.clients-ccloud).

1. Determine which of the files you need:

   * [Java client to Confluent Cloud](clients/cloud/java.config)
   * [Java client to Confluent Cloud with Confluent Cloud Schema Registry](clients/cloud/java-sr.config)
   * [librdkafka-based client to Confluent Cloud](clients/cloud/librdkafka.config)
   * [librdkafka-based client to Confluent Cloud with Confluent Cloud Schema Registry](clients/cloud/librdkafka-sr.config)

2. Copy the file locally.

3. Customize the file with connection information to your Kafka cluster. Notice that the file cannot be used as-is because it has parameters that need to be substituted with real values.  You need to modify the file to provide the values for the bootstrap server and API key and secret. Here is how to create or find [those values](https://docs.confluent.io/current/cloud/using/config-client.html#librdkafka-based-c-clients?utm_source=github&utm_medium=demo&utm_campaign=ch.examples_type.community_content.clients-ccloud).

5. (optional) If you are using a librdkafka-based client, additional configuration properties are supported. See [CONFIGURATION.md](https://github.com/edenhill/librdkafka/blob/master/CONFIGURATION.md) for the full list.		
