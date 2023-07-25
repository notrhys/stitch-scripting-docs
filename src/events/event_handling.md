# Event Handling

**Note:** This is a work in progress, not all events are documented yet.

### Listening for events:

```js
let module = client.registerModule("Name", "Description", "Category")

module.onEnable(() => {

})

module.onDisable(() => {

})

module.events.onGameLoop(() => {

})

module.events.onGameTick(() => {

})

module.events.onPlayerMotion((event) => {

})

module.events.onPlayerMove((event) => {

})

module.events.onPlayerMoveFlying((event) => {

})

module.events.onRender((event) => {

})
```