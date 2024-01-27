<h1>A message queue is a form of communication between different software components or systems. It is widely used in distributed systems to enable asynchronous communication and decouple different parts of a system. The basic idea is to allow one part of a system to send a message to another part without requiring the sender to wait for an immediate response.</h1>

<h1>To Install the dependency</h1>
<h2>npm i govqueue</h2>

<h1>Features of Message Queue</h1>

<h2>getDataStructure()</h2>
<p><strong>Description:</strong> Returns the current data structure of the message queue ('queue' or 'stack').</p>
<p><strong>Parameters:</strong> None.</p>
<p><strong>Returns:</strong> A string representing the current data structure.</p>

<h2>registerProvider(serviceName, callback)</h2>
<p><strong>Description:</strong> Registers a message provider for a specific service.</p>
<p><strong>Parameters:</strong></p>
<ul>
  <li><strong>serviceName (string):</strong> The name of the service.</li>
  <li><strong>callback (function):</strong> The callback function to be executed when messages are provided by the service.</li>
</ul>

<h2>unregisterProvider(serviceName)</h2>
<p><strong>Description:</strong> Unregisters a message provider for a specific service.</p>
<p><strong>Parameters:</strong></p>
<ul>
  <li><strong>serviceName (string):</strong> The name of the service to unregister.</li>
</ul>

<h2>registerConsumer(serviceName, topic, callback)</h2>
<p><strong>Description:</strong> Registers a message consumer for a specific service and topic.</p>
<p><strong>Parameters:</strong></p>
<ul>
  <li><strong>serviceName (string):</strong> The name of the service.</li>
  <li><strong>topic (string):</strong> The topic for which the consumer is registered.</li>
  <li><strong>callback (function):</strong> The callback function to be executed when messages are available for the service and topic.</li>
</ul>

<h2>unregisterConsumer(serviceName, topic, callback)</h2>
<p><strong>Description:</strong> Unregisters a message consumer for a specific service and topic.</p>
<p><strong>Parameters:</strong></p>
<ul>
  <li><strong>serviceName (string):</strong> The name of the service.</li>
  <li><strong>topic (string):</strong> The topic for which the consumer is unregistered.</li>
  <li><strong>callback (function):</strong> The callback function to be unregistered.</li>
</ul>

<h2>addMessage(topic, message, priority = 0)</h2>
<p><strong>Description:</strong> Adds a new message to the message queue or stack.</p>
<p><strong>Parameters:</strong></p>
<ul>
  <li><strong>topic (string):</strong> The topic to which the message belongs.</li>
  <li><strong>message (any):</strong> The content of the message.</li>
  <li><strong>priority (number, optional):</strong> The priority of the message (default is 0).</li>
</ul>

<h2>sortQueueByPriority()</h2>
<p><strong>Description:</strong> Sorts the messages in the queue based on their priority.</p>

<h2>trimDataStructure()</h2>
<p><strong>Description:</strong> Trims the size of the message queue or stack to meet the specified maximum size.</p>

<h2>acknowledgeMessage(messageId)</h2>
<p><strong>Description:</strong> Acknowledges and removes a message from the message queue or stack based on its ID.</p>
<p><strong>Parameters:</strong></p>
<ul>
  <li><strong>messageId (string):</strong> The ID of the message to be acknowledged.</li>
</ul>
<p><strong>Returns:</strong> A string indicating the acknowledgment result.</p>

<h2>dequeueMessages()</h2>
<p><strong>Description:</strong> Dequeues and returns messages from the message queue or stack.</p>
<p><strong>Returns:</strong> An array of messages that have been dequeued.</p>

<h2>startDequeueProcess()</h2>
<p><strong>Description:</strong> Starts the automatic dequeue process at a specified interval. Stops automatically if the queue is empty.</p>
<p><strong>Note:</strong> Adjust the interval as needed based on your application's requirements.</p>

<h2>generateUniqueMessageId()</h2>
<p><strong>Description:</strong> Generates a unique message ID using the uuid library.</p>
<p><strong>Returns:</strong> A unique message ID.</p>









<h1>Code Implementation </h1>

![ray-so-export](https://github.com/Govind-Upadhyay-12/Message_Queue_npm_package/assets/119063599/b8c4064d-4872-4790-90ac-6ecb68a19ca9)

