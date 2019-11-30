# fetchthe-datafromongo
import pymongo
uri = "mongodb://127.0.0.1:27017"
connection =pymongo.MongoClient(uri)
database = connection['gla']
collection = database['student1']
cursor =collection.find()
for i in cursor:
    print(i)
'''data =[
