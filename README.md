# LINE Hospital Integration System

Webhook-based integration platform connecting hospital backend systems with LINE Official Account to enable automated, structured patient communication in production healthcare environments.

---


## Impact

* Automated patient messaging workflows, reducing manual response workload
* Improved response time for common patient requests
* Enabled scalable patient communication through LINE platform
* Provided structured access to hospital services via messaging interface
* Used in real-world healthcare operations

---

## Problem

Hospital staff previously handled patient requests manually through messaging channels, including:

* Appointment inquiries
* Telemedicine access requests
* General hospital information

This resulted in:

* High administrative workload
* Slow response times
* Inconsistent communication quality
* Limited scalability of patient support

---

## Solution

Designed and implemented a webhook-based integration system:

* Connected LINE Official Account to backend services
* Handled incoming patient messages via webhook endpoint
* Delivered structured responses using Flex Messages
* Provided service navigation via Rich Menu interface
* Enabled automated patient workflows for common use cases

---


## Architecture

Message flow:

```id="line_arch"
[Patient]
    ↓
[LINE Official Account]
    ↓
[Webhook (Node.js)]
    ↓
[Message Processing Logic]
    ↓
[Flex Message Response]
```

### Key Considerations

* Designed for **high-frequency messaging scenarios**
* Ensured consistent and structured responses
* Optimized for usability via messaging interface
* Integrated seamlessly with existing hospital workflows

---

## Technical Highlights

* Webhook-based event handling for real-time message processing
* Structured message design using LINE Flex Messages (JSON)
* Integration with external messaging platform (LINE API)
* Modular handling of different message types and workflows

---

## Features

* Automated patient messaging workflows
* Structured responses using Flex Messages
* Service navigation via LINE Rich Menu
* Webhook-based system integration

---

## Tech Stack

* Node.js
* JavaScript
* LINE Messaging API
* Flex Messages (JSON)

---

## Project Structure

```id="line_struct"
flex_message/   JSON templates for structured responses  
push_message/   outbound messaging and notification logic  
richmenu/       configuration and assets for LINE Rich Menu  
route.js        webhook entry point and request routing  
```

---

## Design Decisions

* **Webhook-based architecture**

  * Enables real-time handling of incoming patient messages
  * Scales naturally with messaging volume

* **Structured messaging (Flex Messages)**

  * Ensures consistent UI/UX for patients
  * Supports complex interaction flows

* **Rich Menu navigation**

  * Simplifies access to hospital services
  * Reduces friction for non-technical users

---

## Challenges

* Designing structured message flows within messaging constraints
* Handling diverse patient requests through limited UI
* Ensuring consistent response behavior across different scenarios
* Integrating messaging workflows with existing hospital services

---

## Future Improvements

* Add user state management for multi-step workflows
* Integrate authentication for personalized services
* Expand service coverage (appointments, records, notifications)
* Improve monitoring and logging for message flows

---

## License

MIT
