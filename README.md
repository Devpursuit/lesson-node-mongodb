# 🛢️ Connect MongoDB with Mongoose

Time to store your data! Let’s connect your Express server to MongoDB using Mongoose.

## 🔧 What You’ll Do

- Set up Mongoose.
- Connect to MongoDB.
- Create a basic model and schema.

## ✅ Activity Instructions

1. Install Mongoose:

```
npm install mongoose

```

2. Add this to your `server.js`:

```js
const mongoose = require('mongoose');

mongoose.connect('your-mongodb-uri')
  .then(() => console.log('MongoDB connected'))
  .catch(err => console.error(err));
```

3. Create a model:

```js

const User = mongoose.model('User', {
  name: String,
  email: String
});
```

# 🎯 Success Criteria

* You connected to MongoDB without errors.

* You created and used a Mongoose model.

* You saved or retrieved data!

# 📌 Tip
Use MongoDB Atlas for your cloud database, or Gitpod’s local MongoDB if set up.
