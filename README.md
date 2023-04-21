### Создвние базы данных

```javascript
./bin/mongo liblary
```

### Создвние коллекции

```javascript
db.createCollection('books');
```

### Запрос для _вставки_ данных о двух книгах в коллекцию **books**

```javascript
db.books.insertMoney([
  {
    title: 'string',
    description: 'string',
    authors: 'string',
  },
  {
    title: 'string',
    description: 'string',
    authors: 'string',
  },
]);
```

### Запрос для поиска полей документов коллекции books по полю title

```javascript
db.books.find({ name: { $in: ['title'] } });
```

### Pапрос для _редактирования_ полей: _description_ и _authors_ коллекции **books** по _\_id_ записи

```javascript
db.books.updateOne(
  { _id: 'id' },
  { $set: { description: 'newString', authors: 'newString' } }
);
```
