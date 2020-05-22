# babel-plugin-transform-react-children-function

Transform React Element Children to function children, use as babel-plugin.

### install
```
npm i --save-dev babel-plugin-transform-react-children-function
```

### Example

in 
```
<Observer>
  <div>this message</div>
<Observer>
```

out
```
<Observer>
  {()=> <div>this message</div>}
<Observer>
```

config

```
{
  "plugins": [
      [
        "babel-plugin-transform-react-children-function",
        { tagName: "Observer" }
      ]
    ]
}
```