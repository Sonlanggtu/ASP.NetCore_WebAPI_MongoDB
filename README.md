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
	
https://user-images.githubusercontent.com/40542726/61180316-bcf70800-a63e-11e9-8771-0a41909dc2b4.PNG


######################################################### 
Resource : https://docs.microsoft.com/en-us/aspnet/core/tutorials/first-mongo-app?view=aspnetcore-2.2&tabs=visual-studio-mac 
