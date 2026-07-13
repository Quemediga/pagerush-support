# Component: Alert

## Purpose
Displays a highlighted message box to draw attention to important information.

## When to Use
* Providing tips or extra information (`info`).
* Warning users about potential issues (`warning`).
* Confirming a successful action (`success`).
* Highlighting errors or critical problems (`error`).

## How to Use (Options / Props)

The main message goes between the opening `<Alert>` and closing `</Alert>` tags.

| Option (`prop`) | Description                                  | Required? | Example Value(s)                  |
| :-------------- | :------------------------------------------- | :-------- | :-------------------------------- |
| `type`          | The style/color of the alert box.            | Yes       | `info`, `warning`, `success`, `error` |
| `title`         | An optional bold title at the start of the alert. | No        | `" Heads Up!"`, `"Success!"`      |
| `children`      | The main message text inside the alert box.   | Yes       | Put text between tags            |

## Example MDX Usage

**Informational Alert:**
```mdx
<Alert type="info" title="Did You Know?">
  You can customize your dashboard settings in the profile section.
</Alert>
```

**Warning Alert:**
```mdx
<Alert type="warning">
  Please save your changes before navigating away from this page.
</Alert>
```

**Success Alert:**
```mdx
<Alert type="success" title="Profile Updated">
  Your changes have been saved successfully.
</Alert>
```

**Error Alert:**
```mdx
<Alert type="error" title="Upload Failed">
  The selected file format is not supported. Please upload a JPG or PNG file.
</Alert>
```
