# PageUP GEL Snippets for VS Code

## Available Commands

`pugcontainer`

```ts
import { container } from "@pageup/gel/src/components/core";
import { css } from "./style.css.js";

export const {} = container(
  "",
  (z) => ({}),
  (props) => {
    return <div></div>;
  }
);
```

`pugcomponent`

```ts
import { component } from "@pageup/gel/src/components/core";
import { css } from "./style.css.js";

export const {} = component(
  "",
  (z) => ({}),
  (props) => {
    return <div></div>;
  }
);
```

`pugpage`

```ts
import { page } from "@pageup/gel/src/components/core";
import { css } from "./style.css.js";

export const {} = page(
  "",
  (z) => ({}),
  (props) => {
    return <div></div>;
  }
);
```

`pugcontainerx`

```ts
import { containerX } from "@pageup/gel/src/components/core";
import { css } from "./style.css.js";

interface Props {}

export const {} = containerX<Props>()(
  "",
  (z) => ({}),
  (props) => {
    return <div></div>;
  }
);
```

`pugcomponentx`

```ts
import { componentX } from "@pageup/gel/src/components/core";
import { css } from "./style.css.js";

interface Props {}

export const {} = componentX<Props>()(
  "",
  (z) => ({}),
  (props) => {
    return <div></div>;
  }
);
```

`pugpagex`

```ts
import { pageX } from "@pageup/gel/src/components/core";
import { css } from "./style.css.js";

interface Props {}

export const {} = pageX<Props>()(
  "",
  (z) => ({}),
  (props) => {
    return <div></div>;
  }
);
```

`pugcx`

```ts
import { cx, styleExportProvider } from "@pageup/gel/src/styling";

const container = cx({});

export const { css } = styleExportProvider({
  container,
});
```
