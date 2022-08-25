# Fetch
```js
const getTodos = async () => {
    try{
        const response = await fetch("http://localhost:5000/todos");
        const jsonData = await response.json();
    }catch(err){

    }
}
```
# Post
```js
<input onChange = {e => setDescription(e.target.value)} />

const post = async e => {
    e.preventDefault()
    try{
        const body = {description}
        const response = await fetch("http://localhost:5000/todos",{
            method:"POST",
            headers:{"Content-type":"application/json"},
            body: JSON.stringify(body)
        });
    }catch(err){

    }
}
```