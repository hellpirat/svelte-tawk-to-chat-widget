
# svelte-tawk-to-chat-widget

A component for chat widget [tawk.to]

Example: [example]

## Basic usage

```bash
npm install svelte-tawk-to-chat-widget // or  yarn add svelte-tawk-to-chat-widget
```

 ```js
import { SvelteTawkToChaTWidget } from 'svelte-tawk-to-chat-widget'
// sapper import
import SvelteTawkToChaTWidget from 'svelte-tawk-to-chat-widget/src/TawkToChatWidget.svelte'
```

```html
<SvelteTawkToChaTWidget propertyId="property-id" chatId="chat-id" />
```

## Props

prop name            | type                   | default
---------------------|------------------------|-------------------------
`propertyId`              | `string`                 |
`chatId`                | `string`                 | `"default"`


### `propertyId`
This props set a Property ID. You can get your Property Id from  Dashobard.

### `chatId`
This props set a Chat Id. You can get your chat id from Direct Chat Link in your Dashboard.

```https://tawk.to/chat/{propertyId}/{chatId} ```


## Developing/Modifying svelte-tawk-to-chat-widget

*Note that you will need to have [Node.js] installed.*

Install the dependencies...

```bash
cd svelte-tawk-to-chat-widget
npm install // or yarn
```

...then start [Rollup]:

```bash
npm run build // or yarn build
cd example
npm run dev // or yarn dev
```


Navigate to [localhost:5000]. You should see your app running. Edit a component file in `src`, save it, and your browser will reload the page so you can see your changes automatically.

[tawk.to]: https://www.tawk.to/
[Node.js]: https://nodejs.org
[Rollup]: https://rollupjs.org
[localhost:5000]: http://localhost:5000
[example]: https://svelte-tawk-to-chat-widget.now.sh
