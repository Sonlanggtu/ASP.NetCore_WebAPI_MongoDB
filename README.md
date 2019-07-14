# ASP.NetCore_WebAPI_MongoDB
Create a web API with ASP.NET Core and MongoDB Basic


################# Step by Step ########################

B1: setup MongoDB

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
	
id	"5d2ab93dd098815a5b8f6112"
bookName	"Design Patterns"
price	54.93
category	"Computers"
author	"Ralph Johnson"
	
id	"5d2ab93dd098815a5b8f6113"
bookName	"Clean Code"
price	43.15
category	"Computers"
author	"Robert C. Martin"


######################################################### 
Resource : https://docs.microsoft.com/en-us/aspnet/core/tutorials/first-mongo-app?view=aspnetcore-2.2&tabs=visual-studio-mac 