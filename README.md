# End Point

|     No     |     Route                 |     Keterangan                             |
|------------|---------------------------|--------------------------------------------|
|     1.     |     /                     |     Menampilkan   Halaman Home             |
|     2.     |     /dashboard            |     Menampilkan   Halaman Dashboard        |
|     3.     |     /books                |     Menampilkan   Halaman Books            |
|     4.     |     /addBook              |     Menampilkan   Halaman AddBook          |
|     5.     |     /bookDetail/:id       |     Menampilkan   Halaman BookDetail       |
|     6.     |     /users                |     Menampilkan   Halaman User             |
|     7.     |     /userEdit/:id         |     Menampilkan   Halaman UserEdit         |
|     8.     |     /settings             |     Menampilkan   Halaman Setting          |
|     9.     |     /carts                |     Menampilkan   Halaman Cart             |
|     10.    |     /cartsEdit            |     Menampilkan   Halaman CartEdit         |
|     11.    |     /auth/login           |     Menampilkan   Halaman Login            |
|     12.    |     /auth/signin          |     Menampilkan   Halaman Signin           |
|     13.    |     /publishers           |     Menampilkan   Halaman Publisher        |
|     14.    |     /publisherAdd         |     Menampilkan   Halaman PublisherAdd     |
|     15.    |     /publisherEdit/:id    |     Menampilkan   Halaman PublisherEdit    |
|     16.    |     /genres               |     Menampilkan   Halaman Genre            |
|     17.    |     /genreAdd             |     Menampilkan   Halaman GenreAdd         |
|     18.    |     /genreEdit/:id        |     Menampilkan   Halaman GenreEdit        |

# Bash for Sequelize

>> User
>> ```
>> npx sequelize-cli model:generate --name User --attributes fullname:string,phone:integer,address:string,city:string,image:string
>> ```

>> Book
>> ```
>> npx sequelize-cli model:generate --name Book --attributes pub_id:integer,title:string,price:integer,image:string,desc:string
>> ```

>> BookGenre
>> ```
>> npx sequelize-cli model:generate --name BookGenre --attributes book_id:integer,gen_id:integer
>> ```

>> Genre
>> ```
>> npx sequelize-cli model:generate --name Genre --attributes genre:string
>> ```

>> Publisher
>> ```
>> npx sequelize-cli model:generate --name Publisher --attributes pub_name:string,address:string
>> ```

>> Cart
>> ```
>> npx sequelize-cli model:generate --name Cart --attributes user_id:integer,book_id:integer,quantity:integer
>> ```

>> Auth
>> ```
>> npx sequelize-cli model:generate --name Auth --attributes username:string,email:string,password:string,role:integer,user_id:integer
>> ```
