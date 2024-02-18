yay -S kafka
sudo systemctl kafka.service start
kafka-console-producer.sh --broker-list localhost:9092 --topic test-topic
kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic test-topic --from-beginning

