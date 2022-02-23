# Fetch

## Options

Fetch will take a URL as its first arugement, and then there's an optional second argument, which is anobject, that you can supply to it. So the object will basically
tell fetch how to make a certain kind of request-- it uses specificy object keys to do that (see docs here)[https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch].

```js
{
    method: 'POST', // will default to GET
    headers: {
      'Content-Type': 'application/json'
    },
    body: JSON.stringify(data) // body data type must match "Content-Type" header
}
```

>  Gotcha Alert

`JSON.stringify` is required here to convert the data into an HTTP protocol-compatiable data-encoding (a string).

