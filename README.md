![image](images/confluent-logo-300-2.png)

# About

Template configuration files for Apache Kafka® clients and Confluent Platform components.

# How to use these template files

## With Confluent Cloud

These instructions are for users who need template files with client application configurations for [Confluent Cloud](https://www.confluent.io/confluent-cloud/?utm_source=github&utm_medium=demo&utm_campaign=ch.examples_type.community_content.clients-ccloud).

1. Select which file you need based on the client type:

   * [Java-based client](clients/cloud/java.config) or [Java-based client with Confluent Cloud Schema Registry](clients/cloud/java-sr.config): e.g., Java, Groovy, Kotlin, Scala, Clojure
   * [librdkafka-based client](clients/cloud/librdkafka.config) or [librdkafka-based client with Confluent Cloud Schema Registry](clients/cloud/librdkafka-sr.config): e.g., Python, Go, Ruby, Node, kafkacat, .NET, C
   * [Confluent Platform component](clients/cloud/java.config) or [Confluent Platform component with Confluent Cloud Schema Registry](clients/cloud/java-sr.config): e.g., Confluent CLI, Apache Kafka commands, kafka-connect-datagen, ksql-datagen 

2. Copy the file locally.

3. Customize the file with connection information to your Kafka cluster. Notice that the file cannot be used as-is because it has parameters that need to be substituted with real values.  You need to modify the file to provide the real values for the following parameters. (Here is how to create or find [those values](https://docs.confluent.io/current/cloud/using/config-client.html#librdkafka-based-c-clients?utm_source=github&utm_medium=demo&utm_campaign=ch.examples_type.community_content.clients-ccloud))

  * Required:

    * `{{ BROKER_ENDPOINT }}`
    * `{{ CLUSTER_API_KEY }}`
    * `{{ CLUSTER_API_SECRET }}`

  * Required if using Confluent Cloud Schema Registry:

    * `{{ SR_API_KEY }}`
    * `{{ SR_API_SECRET }}`
    * `{{ SR_ENDPOINT }}`

4. (optional) If you are using a librdkafka-based client, additional configuration properties are supported. See [CONFIGURATION.md](https://github.com/edenhill/librdkafka/blob/master/CONFIGURATION.md) for the full list.		

## With Confluent Platform running on localhost

These instructions are for users who need template files with client application configurations for Confluent Platform running on their local machines, often started with `confluent start`.

1. Select which file you need based on the client type:

   * [Java-based client](clients/local/java.config) or [Java-based client with Confluent Schema Registry](clients/local/java-sr.config): e.g., Java, Groovy, Kotlin, Scala, Clojure
   * [librdkafka-based client](clients/local/librdkafka.config) or [librdkafka-based client with Confluent Schema Registry](clients/local/librdkafka-sr.config): e.g., Python, Go, Ruby, Node, kafkacat, .NET, C
   * [Confluent Platform component](clients/local/java.config) or [Confluent Platform component with Confluent Schema Registry](clients/local/java-sr.config): e.g., Confluent CLI, Apache Kafka commands, kafka-connect-datagen, ksql-datagen

2. Copy the file locally.

3. (optional) If you are using a librdkafka-based client, additional configuration properties are supported. See [CONFIGURATION.md](https://github.com/edenhill/librdkafka/blob/master/CONFIGURATION.md) for the full list.
