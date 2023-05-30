# What is Input Element or Tag

> The `<input>` the tag specifies an input field where the user can enter data.  
> The `<input>` element is the most important form element.  
> The `<input>` the element can be displayed in several ways, depending on the type attribute.

# Input type Attribute

> The type attribute specifies the type of `<input>` element to display.  
> If the type attribute is not specified, the default type is "text"

### Syntax

```xml
<input type="value">
```

## Example

<iframe height="300" style="width:100%" src="https://codepen.io/ZuberUstad/embed/poZNmGW?default-tab=html%2Cresult">
  See the Pen <a href="https://codepen.io/ZuberUstad/pen/poZNmGW">
  Input element example</a> by Zuber Ustad (<a href="https://codepen.io/ZuberUstad">@ZuberUstad</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

## Attribute Values

| Type | Description | Syntax | Examples |
| --- | --- | --- | --- |
| button | A push button with no default behavior displays the value of the value attribute, empty by default. | `<input type="button" name="button" value="Button" />` | Example → [Button](https://yari-demos.prod.mdn.mozit.cloud/en-US/docs/Web/HTML/Element/input/_sample_.examplebutton.html) |
| checkbox | A check box allowing single values to be selected/deselected. | `<input type="checkbox" name="checkbox"/>` | Example →[CheckBox](https://yari-demos.prod.mdn.mozit.cloud/en-US/docs/Web/HTML/Element/input/_sample_.examplecheckbox.html) |
| color | A control for specifying a color; opening a color picker when active in supporting browsers. | `<input type="color" name="color"/>` | Example → [color](https://yari-demos.prod.mdn.mozit.cloud/en-US/docs/Web/HTML/Element/input/_sample_.examplecolor.html) |
| date | A control for entering a date (year, month, and day, with no time). Opens a date picker or numeric wheels for a year, month, and day when active in supporting browsers. | `<input type="date" name="date"/>` | Example → [Date](https://yari-demos.prod.mdn.mozit.cloud/en-US/docs/Web/HTML/Element/input/_sample_.exampledate.html) |
| Number | A control for entering a number. Displays a spinner and adds default validation. Displays a numeric keypad in some devices with dynamic keypads. | `<input type="number" name="number"/>` | Example → [Number](https://yari-demos.prod.mdn.mozit.cloud/en-US/docs/Web/HTML/Element/input/_sample_.examplenumber.html) |
| file | A control that lets the user select a file. Use the accept attribute to define the types of files that the control can select. | `<input type="file" accept="image/*, text/*" name="file"/>` | Example → [file](https://yari-demos.prod.mdn.mozit.cloud/en-US/docs/Web/HTML/Element/input/_sample_.examplefile.html) |
| range | A control for entering a number whose exact value is not important. Displays as a range widget defaulting to the middle value. Used in conjunction with min and max to define the range of acceptable values. | `<input type="range" name="range" min="0" max="25"/>` | Example → [range](https://yari-demos.prod.mdn.mozit.cloud/en-US/docs/Web/HTML/Element/input/_sample_.examplerange.html) |
| password | A single-line text field whose value is obscured. Will alert the user if the site is not secure. | `<input type="password" name="password"/>` | Example → [password](https://yari-demos.prod.mdn.mozit.cloud/en-US/docs/Web/HTML/Element/input/_sample_.examplepassword.html) |

# Resources

[Javapoint](https://www.javatpoint.com/css-position) [W3school](https://www.w3schools.com/) [MDN](https://developer.mozilla.org/en-US/)