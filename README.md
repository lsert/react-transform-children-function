# react-transform-children-function

Transform React Element Children to function children, use as babel-plugin.


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
        "@babel/plugin-transform-react-children-function",
        { tagName: "Observer" }
      ]
    ]
}
```