# express-node-snippets

## Express

### Middleware

#### HTTP Reqest Logger
```
const logger = (req, res, next) => {
  console.log(`${req.method} ${req.protocol}://${req.get('host')}${req.originalUrl}`)
  next();
}
```
