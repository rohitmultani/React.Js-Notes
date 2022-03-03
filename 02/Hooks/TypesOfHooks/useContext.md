# useContext

This is helpful in sharing state between siblings components, as props value cannot be passed between the siblings rather they have to go with the tree structure, and if a state is required deep inside a branch it should be pass through all its parent component.
To remove this useContext is introduced.

## Create Context 
To create context, you must Import createContext and initialize it:
```
import { useState, createContext } from "react";
const UserContext = createContext({default object});
export default UserContext;
```

Now we had created context, which we can use as Context Provider to wrap the tree structure where that state is needed

## Context Provider
```
<UserContext.Provider>
<DummyComponent value={changed object}/>
</UserContext.Provider>
```

## Consuming or Using the Conntext

cont anyVariable = useContext(UserContext);

## Limitations
 React Context is not optimized for high frequency changes.
 to overcome this Redux is there.