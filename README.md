# PageUP GEL Snippets for VS Code

## Available Commands

`pugcontainer`

```ts
import { container } from "@pageuppeopleorg/gel/src/components/core";
import { css } from "./styles.css";

export const { Sample } = container(
  "Sample",
  (z) => ({
    name: z.string(),
  }),
  (props) => {
    return <div>{props.name}</div>;
  }
);
```

`pugcomponent`

```ts
import { component } from "@pageuppeopleorg/gel/src/components/core";
import { css } from "./styles.css";

export const { Sample } = component(
  "Sample",
  (z) => ({
    name: z.string(),
  }),
  (props) => {
    return <div>{props.name}</div>;
  }
);
```

`pugpage`

```ts
import { page } from "@pageuppeopleorg/gel/src/components/core";
import { css } from "./styles.css";

export const { Sample } = page(
  "Sample",
  (z) => ({
    name: z.string(),
  }),
  (props) => {
    return <div>{props.name}</div>;
  }
);
```

`pugcontainerx`

```ts
import { containerX } from "@pageuppeopleorg/gel/src/components/core";
import { css } from "./styles.css";

interface Props {
  name: string;
}

export const { Sample } = containerX<Props>()(
  "Sample",
  (z) => ({
    name: z.string(),
  }),
  (props) => {
    return <div>{props.name}</div>;
  }
);
```

`pugcomponentx`

```ts
import { componentX } from "@pageuppeopleorg/gel/src/components/core";
import { css } from "./styles.css";

interface Props {}

export const { Sample } = componentX<Props>()(
  "Sample",
  (z) => ({
    name: z.string(),
  }),
  (props) => {
    return <div>{props.name}</div>;
  }
);
```

`pugpagex`

```ts
import { pageX } from "@pageuppeopleorg/gel/src/components/core";
import { css } from "./styles.css";

interface Props {}

export const { Sample } = pageX<Props>()(
  "Sample",
  (z) => ({
    name: z.string(),
  }),
  (props) => {
    return <div>{props.name}</div>;
  }
);
```

`pugcx`

```ts
import { cx, styleExportProvider } from "@pageuppeopleorg/gel/src/styling";

const container = cx({});

export const { css } = styleExportProvider({
  container,
});
```
