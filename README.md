# A Package that simplifies the implementation publish-subscribe architecture methodology

## Overview
Pub/Sub is a lightweight Publish-Subscribe architecture implementation for enhancing data flow between components in various applications. It allows components to communicate effectively without direct dependencies, promoting modularity and scalability.

## Implementation
https://medium.com/@karandeepsinghworkspace/efficient-data-sharing-in-react-a-deep-dive-into-pub-sub-architecture-3af5362bd8c9

## Features
- **Publish**: Broadcast messages or data to multiple subscribers.
- **Subscribe**: Receive and react to specific messages or events.
- **Unsubscribe**: Remove subscriptions when no longer needed.

## Installation
You can install Pub/Sub via npm:

```bash
npm i viewlift-pubsub

```javascript
import PubSub from '@your-package/pubsub';

const callback = (data) => {
  console.log('Received:', data);
};

// Subscribe to an event
PubSub.subscribe('event-name', callback);

// Publish data to subscribers
PubSub.publish('event-name', { message: 'Hello, world!' });

// Unsubscribe when done
PubSub.unsubscribe('event-name', callback);
```