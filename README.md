# JSON SERVER [Click to open the documentation](https://github.com/typicode/json-server)

# Steps
```sh
> npm install
> npm run server
```

### **Get All Users**
```
 - http://localhost:3000/users
```

### **Get All Companies**
```
 - http://localhost:3000/companies
```

### **Get Single User**
```
 - http://localhost:3000/users/1
```

### **Get Single Company**
```
 - http://localhost:3000/companies/1
```

### **Get All Users Of a Company**
```
 - http://localhost:3000/companies/1/users
```

### **Filter Companies By Name**
```
- http://localhost:3000/companies?name=Apple
- http://localhost:3000/companies?name=Microsoft&name=Apple
```

### **Pagination & Limit**
```
 - http://localhost:3000/users?_page=1&_limit=2
```

### **Sorting**
```
- http://localhost:3000/users?_sort=firstname&_order=desc
```

### **FULL Text Searching**
```
- http://localhost:3000/users?q=mich
```

### **Range**
```
- http://localhost:3000/users?age_gte=30
- http://localhost:3000/users?age_gte=30&age_lte=40
```
### **Relationships**
#### *In Companies Many Users Can work*
```
- http://localhost:3000/companies?_embed=users
```
#### *User Belongs To Company*
```
- http://localhost:3000/users?_expand=company
```

### **Authenticate**
> curl -d "token=abcdef-1234-5678" http://localhost:3000/authenticate
```sh
- [POST] http://localhost:3000/authenticate
- [GET] http://localhost:3000/authenticate
```
