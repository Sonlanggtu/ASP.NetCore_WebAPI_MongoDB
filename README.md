# ASP.NetCore_WebAPI_MongoDB
Create a web API with ASP.NET Core and MongoDB Basic


################# Step by Step ########################

B1: Setup MongoDB

B2: open cmd 
     mongod --dbpath <data_directory_path> 

B3: Create DB from MongoDB 
Open cmd:
	mongo
	use BookstoreDb
	db.createCollection('Books')
	db.Books.insertMany([{'Name':'Design Patterns','Price':54.93,'Category':'Computers','Author':'Ralph Johnson'}, {'Name':'Clean Code','Price':43.15,'Category':'Computers','Author':'Robert C. Martin'}])


B4: Test MongoDB table
	db.Books.find({}).pretty()

B5: http://localhost:<port>/api/books

################# Result ##########################
	
![Capture](https://user-images.githubusercontent.com/40542726/61180346-20813580-a63f-11e9-94f9-4f7a63398a6e.PNG)

######################################################### 
Resource : https://docs.microsoft.com/en-us/aspnet/core/tutorials/first-mongo-app?view=aspnetcore-2.2&tabs=visual-studio-mac 
