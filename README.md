# 💮 Desa Ubud Website Using Laravel 💮

## 🖼️ Project Description 
<p align="center">
    <img width="800" src="https://github.com/user-attachments/assets/e4312388-853e-4b1e-abc2-5001db25bd6d">
</p>

**Introduction**

Desa Ubud Website is The Ubud Village Website is a type of village website that provides an overview about Ubud Village, activities/news related to Ubud Village, tourist attractions, and several lodgings located around the village. The website also provides admin page which will manage the content on the website, such as news, objects tours, contacts, and accommodation (in the form of lodging and prices).

**Features**
- **User Registration & Login** 

  User registration is used to stored new user data, while User login is used to verify the user data that has been registered through registration feature. Login's verification uses the 
 _Middleware_ and the _Authentication_ services using library _Auth Facades_. 
- **Searching & Pagination**

  Searching is used to find data easily using related keywords, while Pagination is used to display the appearance of the website so that it looks simple and neat. These features use the _Bootstrap_ framework which provides the required design templates. 
- **Admin Page**

  Admin Page is a special admin feature for managing websites. This feature contains CRUD (Create, Read, Update, & Delete) which helps admins create, update, and delete content in website.

## ⚙️ Setup
**Dependencies**
  - Laravel == 8x
  - Bootstrap == 3.4
  - Composer == 2.0.12
  - PHP == 3.4.0
    
**Tools**
  - VS CODE : as the IDE (you can use another IDE).  
  - XAMPP : software to access MySQL Server for Database.  
  - Browser : for showing up the result (using localhost).

## 🏬 Database Schema 
**Table & Fields**
- Database Name: laravel 
- Total Table: 5 tables

  | Table name | Atributes | Purpose |
  | ---------- | --------- | ------- |
  | accomodation | id, nama, body, image, harga | saving accomodation data | 
  | news | id, author_id, title, slug, excerpt, body, image | saving news data | 
  | comments | id, nama, email, alamat, body | saving comments data |
  | users | id, nama, email, password (has been encrypted) | saving users data |
  | tourism | id, title, excerpt, body, image | saving tourism data |

## 💻 Deployment 
**Cloning Project**
- Open the project on github, find the HTTPS or SSH button. Choose and press one of them, then copy the link provided.
- In your local computer, create or choose the folder you want to save the project. Open the gitbash, type this command ```git clone [paste the link]``` and paste the copied-link after that. If you can't find the gitbash, then you should download and install git or your computer.
  
**Running Project**
- Open the project on your IDE. Copy file .env by using ```cp.env.example .env``` (change the copied-file from .env.example to .env). Make sure the name of databases already exists in your database system.
- Open the terminal section and type this command ```composer install```for installing the Composer.
- Type this command ```php artisan key:generate``` after you there's no doubt in step one and two.
- After that, type this command ```php artisan migrate``` to migrate the all the table's structures to your database.
- This project provides a database seeder to give you a data example, so type this command too ```php artisan db:seed```.
- Finally type this command to run the project ```php artisan serve```.
- Well done!

## 🖋️ Additional Comments 
**Future Plans**:
- Improving the design and features in Admin Page.
- Building a more well-structured database with good and correct table naming.
