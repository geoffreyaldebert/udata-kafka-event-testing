# udata-kafka-event-testing

This repository allow to generate different kind of udata messages for testing purpose. It provides also monitoring for every udata messages sent to Kafka.

### Initialization 

```
pip install -r requirements.txt
pip install .
docker-compose up -d # For launching kafka 
```

### Consume messages

```
udata-kafka-event-testing consume
```

### Produce message

```
udata-kafka-event-testing produce <TOPIC_NAME> <SERVICE_NAME:OPTIONAL> <MESSAGE_TYPE:OPTIONAL>
```

If there is sereral services or message types for a specific topic and you don't wrote it in command, prompt will ask which one you want.

