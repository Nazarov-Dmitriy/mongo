db.collection.insertMany([
  {
    title: "книга1",
    description: "описание книги 1",
    authors: "Автор1"
  
  },
  {
    title: "книга2",
    description: "описание книги 2",
    authors: "Автор1"
  
  }
]);

   
db.collection.find({ title:  "книга1" })

db.collection.update(   
  {_id: 1 },
  { $set: { description: "Новая книга",authors :'Новый автор'} }
);