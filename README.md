# Path Based Component Naming
A consistent way to name your components


# Motivation
Currently, there's no standard way to name components in a React project. If you don't have a pattern while working in a team, it's very likely that your component names will get messy. You end up repeating names in your files and your imports constantly become to big to fit in a single row. You can avoid that scenario by following some simple rules:

### All the components should be named accordingly to its relative path to folder `components`, or `src` if you are outside `components`
> By named, we mean the component name and not the file name. Or be, the name you give to your class or to the const you assigned your component:
```js
class MyComponent extends Component {
}
const MyComponent () => {};
```
A component located at `src/components/User/List.jsx` would be named as `UserList`, but a component located at `src/screens/User/List.jsx`, would be named as `ScreensUserList`.

**Why?**
Naming components that way, will help you locate your component by just looking into it's name. If you have fuzzy search for example, you can just copy and paste the component's name and your editor will give you the proper file:

It's also very easy to locating your component navigating in the folder's tree:

### Omit file name when the component is inside a folder with it's own file name
`src/components/User/List/List.jsx ->  UserList`

`src/screens/User/List/List.jsx ->  ScreensUserList`

### Name component files only accordingly to its context

