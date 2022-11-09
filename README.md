

1. запрос(ы) для вставки данных минимум о двух книгах в коллекцию books

db.books.insertMany([{title:'Книга1', description: 'Описание 1', authors: 'Автор 1'},
{title:'Книга2', description: 'Описание 2', authors: 'Автор 2'}])

2. запрос для поиска полей документов коллекции books по полю title 

db.books.find({title:'Книга2'})

3. запрос для редактирования полей: description и authors коллекции books по _id записи

db.books.updateOne({_id:'указываем нужный id'}, {$set{
    description:'Описание 4',
    authors:'Автор 4'
}})