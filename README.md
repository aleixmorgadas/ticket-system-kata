# ticket-system-kata

Practicing the temporal order of a ticket system.

## What should you expect from this kata?

The kata is meant to be done in 3 or more consecutive sessions.

1. [**Session I**. Domain Discovery][session-1].

Analysis phase. We will use different techniques to find the essential domain complexity and draw the different bounded contexts.

2. [**Session II**. Domain Implementation][session-2].

3. [**Session III**. Validating Architectural decisions using persistance layers. A real environment][session-3].

### Starting Technologies

- Java 11
- Gradle
- JUnit 5
- [Spring Boot 2][springboot]
- Docker & Docker Compose

### Practices

- Test-Driven Development
- Continuous Integration

For Domain analysis and discovery, we might practice:

- [Event Storming][eventstorming]
- [Domain Storytelling][domainstorytelling.org]

## Domain

We are working in a famous old museum, which attracts a lot of tourists each day. The demand is high and few space available compared.

### Problem Space

The stakeholders want to create a ticket system that matches the current way the museum has to sell tickets as a value proposition, in order to attend you can only buy a ticket the same day. Instead of selling the tickets upfront, we want to sell the tickets for the same day starting at 9:00 local time online.

Since the demand is high and the space available reduced, the stakeholders asked to emulate how selling the ticket happens in the real world with the online shop, with a virtual queue which guarantees the order of arrival.

![queue-diagram][queue-diagram]

### High level system behavior using Domain Storytelling

![storytelling][storytelling]

:information_source: You can use the [domain storytelling online tool][wps] with the [file used to generate the diagram](wps-file).

1. See available tickets
2. Queue number
3. Buy ticket
4. Ticket

[session-1]: ./doc/kata-runbooks/session-1.md
[session-2]: ./doc/kata-runbooks/session-2.md
[session-3]: ./doc/kata-runbooks/session-3.md
[queue-diagram]: ./doc/supporting-images/queue-diagram.png
[storytelling]: ./doc/supporting-images/storytelling.svg
[domainstorytelling.org]: https://domainstorytelling.org/
[eventstorming]: https://www.eventstorming.com/
[springboot]: https://spring.io/projects/spring-boot
[wps]: https://www.wps.de/modeler/
[wps-file]: ./doc/supporting-images/storytelling.dst
