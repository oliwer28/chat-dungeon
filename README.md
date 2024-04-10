# chat-dungeon

The chat app made for dungeon dwellers. 

Dig into those deep conversations.

## Architecture

```mermaid
zenuml
    try {
      Consumer->API: Book something
      API->BookingService: Start booking process
    } catch {
      API->Consumer: show failure
    } finally {
      API->BookingService: rollback status
    }

```