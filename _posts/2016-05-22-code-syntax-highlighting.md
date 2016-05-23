---
layout: post
title: Code Syntax highlighting
---
# Introduction

Using standard backticks

```
@Bean
TopicExchange exchange() {
	return new TopicExchange(AmqpSettings.DMF_EXCHANGE);
}

@Bean
Binding binding(Queue queue, TopicExchange exchange) {
	return BindingBuilder.bind(queue).to(exchange).with(queueName);
}

@Bean
SimpleMessageListenerContainer container(ConnectionFactory connectionFactory, MessageListenerAdapter listenerAdapter) {
	SimpleMessageListenerContainer container = new SimpleMessageListenerContainer();
	container.setConnectionFactory(connectionFactory);
	container.setQueueNames(queueName);
	container.setMessageListener(listenerAdapter);
	return container;
}
```

Using backticks with language

```java
@Bean
TopicExchange exchange() {
	return new TopicExchange(AmqpSettings.DMF_EXCHANGE);
}

@Bean
Binding binding(Queue queue, TopicExchange exchange) {
	return BindingBuilder.bind(queue).to(exchange).with(queueName);
}

@Bean
SimpleMessageListenerContainer container(ConnectionFactory connectionFactory, MessageListenerAdapter listenerAdapter) {
	SimpleMessageListenerContainer container = new SimpleMessageListenerContainer();
	container.setConnectionFactory(connectionFactory);
	container.setQueueNames(queueName);
	container.setMessageListener(listenerAdapter);
	return container;
}
```

Using ```highlights```

{% highlight java %}
@Bean
TopicExchange exchange() {
	return new TopicExchange(AmqpSettings.DMF_EXCHANGE);
}

@Bean
Binding binding(Queue queue, TopicExchange exchange) {
	return BindingBuilder.bind(queue).to(exchange).with(queueName);
}

@Bean
SimpleMessageListenerContainer container(ConnectionFactory connectionFactory, MessageListenerAdapter listenerAdapter) {
	SimpleMessageListenerContainer container = new SimpleMessageListenerContainer();
	container.setConnectionFactory(connectionFactory);
	container.setQueueNames(queueName);
	container.setMessageListener(listenerAdapter);
	return container;
}
{% endhighlight %}


Using gists

<script src="http://gist.github.com/93348a9ddf55d0ddb0f0ac6c153e4a8e.js"></script>