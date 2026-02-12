# PubNub-latency-demo
Simple demo to measure latency of one or multiple browser clients

## Details

User clicks one of the provided color buttons causing the backgroundColor to be changed on every open session of this file utilizing the same pub/sub keys & channel. The click event sends a message payload to PubNub consisting of the color selection, and `sentAt` time the message is being sent. Subscribers receive this message, change their backgroundColor, then display the latency (determined by deducting the `sentAt` time from local time).


## Config

Replace     
```
publishKey: "pub-key-here"
subscribeKey: "sub-key-here"
```

with your pub/sub keys


## Todo List

1. Display all users that currently have the page open
2. Display latency results for all users

