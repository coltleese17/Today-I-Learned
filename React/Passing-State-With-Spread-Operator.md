# Passing State With Spread Operator

When passing down state, e.g. from a smart component to a presentational component for rendering, you can either send it a single object containing state, e.g. :
```
render() {
        <FormComponent
            handleChange={this.handleChange}
            data={this.state}
        />
    }
```

which is accessed via `props.data.propertyName`.

Or you can use the spread operator to pass down the state e.g. :

```

render() {
        <FormComponent
            handleChange={this.handleChange}
            {...this.state}
        />
    }
```

which is accessed via the cleaner `props.propertyName`.
