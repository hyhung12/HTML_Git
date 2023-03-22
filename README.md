- HTML defines content + structure of the website

    ```
    <HTML element HTML attribute>
    ```
    
- HTML boilerplate (saved as abc.html extension and presing ! in VSCode) -> like a hamburger

    ```
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>

    </body>
    </html>
    ```
    
-> HTML is about adding element tag
```
-                     1.
-                     2.
-                     3.
```
unordered list    &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  ordered list
-> Make coding as habit

- CSS: change font, color
- Responsive: different layouts for different platform(mobile, desktop) == Adaptive layout
```
.gitignore -> don't upload files to GitHub
git branch -> check available branches
git checkout <new_branch> -> move to new branch
git merge <branch_to_merge>

git remote add origin https://github.com/hyhung12/Test_Repo3.git
git push -u origin main
```
- Update method
```
db.<collection_name>.updateOne({_id:1}, {$set: {stock:32}})
```
- One-to-many (one product with many reviews, one user with many comments)
- Delete a database: switch to database
```
db.dropDatabase()
```
```
const mongoose = require('mongoose');
mongoose.connect('mongodb://0.0.0.0:27017/fruitsDB');

const fruitSchema = new mongoose.Schema ({
    name: String,
    rate: Number,
    review: String
});

const Fruit = mongoose.model('Fruit', fruitSchema);

const fruit = new Fruit ({
    name: "Apple-2",
    rating: 7,
    review: "apple is apple"
});

fruit.save();
Fruit.insertMany([kiwi, orange, banana], function(err){
if (err){console.log('error')}else{console.log('successful')}});
Fruit.find(function(err, fruits){if (err){console.log('error')}else{console.log(fruits)}});
```

