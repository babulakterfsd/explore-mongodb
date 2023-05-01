# MongoDB : let's dive deep into it...

#### mongo: This command opens the MongoDB shell.

1. use db -> change database
2. show collections -> will show collections in current db
3. db.users.find() -> will show all the documents in the collection
4. db.users.find().count() -> how much data are there in the collection
5. db.users.find({age: 23}) -> 23 bochor boyoshi joto user ache tader dekhabe
6. db.users.find().projection({\_id: 0}) -> shob data dekhabe, kintu \_id property chara. projection e evabe je property deya hobe, seti e mongodb ar pathabe na.

7. db.users.find({age: 23}).projection({\_id: 0}) -> 23 bochorer sob user ashbe, kintu \_id props chara
8. db.users.find({skills: 'JavaScript'}) -> skills ekta array. sekhan theke evabe data ana hocche. jodi full array match korate hpy, tahole ["JavaScript", "Python"] evabe exact array deya lagto. abar nested object thekeo data ana jay. acc er backend er 5 number module e ache.

9. db.users.find({age: {$gt: 23}}) -> 23 bochorer boro shob user ke dekhabe

10. db.users.find().sort({age: -1}) -> age gula upor theke sort hoye dekhabe
