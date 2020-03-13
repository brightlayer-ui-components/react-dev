# InfoListItem
The InfoListItem is intended to be used in List views. It positions a title as well as optional subtitle(s), icon, and status stripe.

<img width="100%" alt="Info List Items in a variety of styles" src="./images/infoListItem.png">

## Usage

```typescript
import { InfoListItem } from '@pxblue/react-components';
import { GradeA, Leaf, CurrentCircled, VoltageCircled, Temp } from '@pxblue/icons-mui';
import * as Colors from '@pxblue/colors';
...
<InfoListItem
    title={'Status'}
    divider={'full'}
    statusColor={Colors.green[500]}
    subtitleSeparator={'/'}
    icon={<Leaf color={'inherit'} />}
/>
```

## API

<div style="overflow: auto;">

| Prop Name         | Description                                      | Type                                               | Required | Default             |
|-------------------|--------------------------------------------------|----------------------------------------------------|----------|---------------------|
| avatar            | Show colored background for icon                 | `boolean`                                          | no       | false               |
| backgroundColor   | The color used for the background                | `string`                                           | no       |                     |
| chevron           | Add a chevron icon on the right                  | `boolean`                                          | no       | false               |
| dense             | Smaller height row with less padding             | `boolean`                                          | no       | false               |
| divider           | Show a row separator below the row               | `'full'` \| `'partial'`                            | no       |                     |
| fontColor         | Title text color                                 | `string`                                           | no       |                     |
| hidePadding       | Remove left padding if no icon is used           | `boolean`                                          | no       | false               |
| icon              | A component to render for the icon               | `React.Component`                                  | no       |                     |
| iconColor         | Color override for the row icon                  | `string`                                           | no       |                     |
| leftComponent     | Component to render on the left side             | `React.Component`                                  | no       |                     |
| onClick           | A function to execute when clicked               | `function`                                         | no       |                     |
| rightComponent    | Component to render on the right side            | `React.Component`                                  | no       |                     |
| ripple            | Whether to apply material ripple effect on click | `boolean`                                          | no       | false               |
| statusColor       | Status stripe and icon color                     | `string`                                           | no       |                     |
| subtitle          | The text to show on the second line              | `string` \| `Array<React.ReactNode>`               | no       |                     |
| subtitleSeparator | Separator character for subtitle                 | `string`                                           | no       | '·' ('\u00B7')      |
| title             | The text to show on the first line               | `string`                                           | yes      |                     |

</div>
