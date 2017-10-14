# Sass scaling mixin

Allows you to scale the interface.

### Install:

```
npm i sass-scaling-mixin
```
```
@import "~sass-scaling-mixin";
```

### Use:
```
.my-class {
    color: red;
    text-align: center;
    
    @include scalingSize((
        font-dize: 20px,
        margin: 20px 10px,
    ))
    
    @include mobileStyles {
        font-dize: 15px,
        margin: 15px 5px,
    }
}
```

or

```
.my-class {
    color: red;
    text-align: center;
    
    @include scalingSize((
        font-dize: 20px,
        margin: 20px 10px,
    ))
}

 @include mobileStyles {
     .my-class {
        font-dize: 15px,
        margin: 15px 5px,
     }
}
```

or

```
.my-class {
    color: red;
    text-align: center;
    
    @include scalingSize((
        font-dize: 20px,
        margin: 20px 10px,
    ))
    
    @include mobileStyles {
        font-dize: 15px,
        margin: 15px 5px,
    }
    
    @media (max-width: 320px) {
        font-dize: 10px,
        margin: 10px 0px,
    }
}
```

