##. Setup
1.1 Creating a new React app
```
    create-react-app blog
```
1.2 Adding the Bootstrap framework
```
    npm install --save bootstrap
```
1.3 Integrating the Bootstrap CSS into index.js
```
    import '../node_modues/bootstrap/dist/css/bootstrap.min.css';
```
1.4 Adding a Bootstrap container into App.js
```
    class App extends Component {
        render() {
            return (
                <div className ="container">
                    <h1>My Blog </h1>
                </div>
            );
        }
    }  
```

##. Implementing the Bootstrap navigation
2.1 Navigation React Component

2.2 Bootstrap navbar
    Copy the content of navbar as found on the Bootstrap documentation page
    class attributes should be renamed to className (use find & replace)
    links should not point to ‘#’ so replace that with /

2.3 Abstracting the NavItem
    abstract the entries in the navbar into a component

2.4 Active NavItem
```
    const liClassName = (props.path === pageURI) ? "nav-item active" : "nav-item";
```

2.5 Disabled NavItem
```
      const aClassName = props.disabled ? "nav-link disabled" : "nav-link"
```

2.6 Using the NavItem

2.7 Adding a NavDropdown

2.8 Adding state to NavDropdown