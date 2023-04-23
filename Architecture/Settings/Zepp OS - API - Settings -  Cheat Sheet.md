## Logging
https://docs.zepp.com/docs/reference/app-settings-api/global/

 ```Javascript
console.log()`
 ```

Console prints a log with any number of parameters.

 ```Javascript
 console.log('Hello Zepp OS')`
 ```

 ```Javascript
 AppSettingsPage({
  build(props) {
    console.log("=== Show the props ===")
    console.log(props)
    return Section({ }) 
  },
})
 ```

## Settings

https://docs.zepp.com/docs/reference/app-settings-api/ui/section/
 ```Javascript
(props: Props, renderFuncArr?: RenderFunc | Array<RenderFunc>) => result: RenderFunc
 ```

## Section

### Type

```javascript
(props: Props, renderFuncArr?: RenderFunc | Array<RenderFunc>) => result: RenderFunc
```

### Props: object

| Name        | Description                                | Required | Type     | Default |
| ----------- | ------------------------------------------ | -------- | -------- | ------- |
| style       | style property, support for CSS attributes | NO       | `object` | -       |
| title       | title of the Section                       | NO       | `string` | -       |
| description | description of Section                     | NO       | `string` | -       |

### Sample

 ```Javascript
AppSettingsPage({
  build(props) {
    return Section({ // https://docs.zepp.com/docs/reference/app-settings-api/ui/section/
      title: "Titel here",
      description: "Description here..."
    }) 
  },
})
 ```

