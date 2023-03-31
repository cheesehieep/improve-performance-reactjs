# Improve-performance-reactjs
- When is component re-rendered?
  + Props changed
  + State changed
  + Parent component re-rendered
  
## Redux
- Example: Only update name of user
  + Component Name display name of user
  + Component Age display age of user
  + Dispatch update name of user from any component

![reducer](https://user-images.githubusercontent.com/62127758/228455102-e30e6a7c-d972-4bc2-9cb7-d29e3425956f.png)

### Class component
![redux-class](https://user-images.githubusercontent.com/62127758/228453807-68a1c9e1-ac8e-447f-a8c9-d0e869b2b032.png)
- Age component re-rendered

![redux-class-unresolve](https://user-images.githubusercontent.com/62127758/228454140-19c06f7a-b2a0-4643-9c99-9f353e40fb4e.png)
- Resolve (Selector exactly state need to be used)

![redux-class-resolve](https://user-images.githubusercontent.com/62127758/228454463-feef5119-af32-4402-bcd5-fb503017145e.png)

### Function component
![redux-re-render](https://user-images.githubusercontent.com/62127758/227871766-6320d5e8-e2df-4082-8ca0-2ca41d197100.png)
- Resolve (Selector exactly state need to be used)

![redux-unresolve](https://user-images.githubusercontent.com/62127758/227873568-9d726157-1e90-4d93-9282-b34dad3a5895.png)
![redux-resolve](https://user-images.githubusercontent.com/62127758/227872810-1f799a5d-3840-4579-ab3e-f0d2a791f1e1.png)

## Context API
![context](https://user-images.githubusercontent.com/62127758/228487050-4503c5b4-d850-4a29-8d47-a488c1ccf425.png)
- Add package `use-context-selector`

![context-unresolve](https://user-images.githubusercontent.com/62127758/228489023-96d011c8-0804-4539-a82d-36da763fe40c.png)

- Resolve 
  + Use package `use-context-selector` and access exactly state need to be used
  + Memo children component (avoid to parent component re-renderd)

![context-resolve](https://user-images.githubusercontent.com/62127758/228487036-b92a77e8-00be-48e2-b90b-9a4002aadead.png)

## React query
![query](https://user-images.githubusercontent.com/62127758/229055588-90b645bf-0cb9-452e-b5e6-92e7850546a3.png)

- Resolve
  + Use option `select` of useQuery to access exactly data need to be used
  + This option can be used to transform or select a part of the data returned by the query function. It affects the returned data value, but does not affect what gets stored in the query cache
  
![query-resolve](https://user-images.githubusercontent.com/62127758/229055692-f895e75c-d2f1-4be7-af96-eb8825377d49.png)




