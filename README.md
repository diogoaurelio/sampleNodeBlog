Notes on console actions needed to be performed:
mongo
use nodeblog;
db.createCollection('posts');
db.createCollection('categories');

db.posts.insert( { title: "Blog post 1", category: "tech", author: "John", body: "This is the body", date: ISODate() } )
db.posts.find().pretty();
db.posts.insert( { title: "Blog post 2", category: "psycology", author: "Susan", body: "This is a Psycology post", date: ISODate() } );
db.posts.find().pretty();

db.categories.insert({ title: "tech" })
db.categories.insert({ title: "Psycology"})
