## Fiddler HW

#### Ex_0: Filter the query output according to the desired id

Protocol: http

IP: 162.55.220.72

Port: 5005

#### Ex_1: 

Method: GET

EndPoint: /get_method

request url params: 
 
 ```
 name: str
 age: int
```

response: 
```
[
    “Str”,
    “Str”
]
```

Task:

Create rules:
 
 - Replace url so that name filled in in Postman is changed in the request.
 - Replace url so that age filled in in Postman is changed in the request.

==================

#### Ex_2:

Method: POST

EndPoint: /user_info_3

request form data: 
```
name: str
age: int
salary: int
```
response: 
```
{'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'u_salary_1_5_year': salary * 4}}
```

Task:

Create rules:
 
 - Replace request body so that name filled in in Postman is changed in the request.
 - Replace request body so that age filled in in Postman is changed in the request.
 - Replace request body so that salary filled in in Postman is changed in the request.
 - Replace request body so that age filled in in Postman is deleted. (Code 500 should be recieved)
 - Change children to neighbors in the response. 
 - Change value of param salary u_salary_1_5_year to another amount in the response.
 - Delete param salary in the response. 

==================

#### Ex_3:

Method: GET

EndPoint: /object_info_1

request url params: 
```
 name: str
 age: int
 weight: int
```
response: 
```
{'name': name,
          'age': age,
          'daily_food': weight * 0.012,
          'daily_sleep': weight * 2.5}
```
Task:

Create rules:
 - Replace url so that name filled in in Postman is changed in the request.
 - Replace url so that age filled in in Postman is changed in the request.
 - Replace url so that salary filled in in Postman is changed in the request.
 - Replace url so that weight filled in in Postman is deleted in the request.
 - Delete param daily_food in the response.
 - Change value of param daily_food to anoher amount in the response.
 - Rename daily_sleep to sleep in the response.
 - Change value of param daily_sleep to another amount in the response.

==================

#### Ex_4:

Method: GET

EndPoint: /object_info_3

request url params: 
```
 name: str
 age: int
 salary: int
```
response: 
```
{'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'pets': {'cat':{'name':'Sunny',
                                     'age': 3},
                              'dog':{'name':'Luky',
                                     'age': 4}},
                     'u_salary_1_5_year': salary * 4}
          }
```

Task:

Create rules:

 - Replace url so that name filled in in Postman is changed in the request.
 - Replace url so that age filled in in Postman is changed in the request.
 - Replace url so that name filled in in Postman is deleted in the request.
 - Delete param salary in the response.
 - Change value of param cat to another json in the response.
 - Recieve code 405.

==================
#### Ex_5:

Method: GET

EndPoint: /object_info_4

request url params: 
```
 name: str
 age: int
 salary: int
```
response: 
```
{'name': name,
          'age': int(age),
          'salary': [salary, str(salary * 2), str(salary * 3)]}
```

Task:
 - Replace url so that name filled in in Postman is changed in the request.
 - Replace url so that age filled in in Postman is changed in the request.
 - Replace url so that salary filled in in Postman is deleted in the request.
 - Delete param salary in the response.
 - Replace value of param salary to value of text type in the response.
 - Recieve code 405.

==================
#### Ex_6:

Method: POST

EndPoint: /user_info_2

request form data: 
```
 name: str
 age: int
 salary: int
```
response: 
```
{'start_qa_salary': salary,
          'qa_salary_after_6_months': salary * 2,
          'qa_salary_after_12_months': salary * 2.7,
          'qa_salary_after_1.5_year': salary * 3.3,
          'qa_salary_after_3.5_years': salary * 3.8,
          'person': {'u_name': [user_name, salary, age],
                     'u_age': age,
                     'u_salary_5_years': salary * 4.2}
          }
```

Task:

Create rules:
 
 - Replace request body so that age filled in in Postman is changed.
 - Replace request body so that salary filled in in Postman is changed.
 - Replace request body so that salary filled in in Postman is deleted.
 - Replace qa_salary_after_6_months to qa_salary_after_10_months in the response.
 - Replace value of salary qa_salary_after_1.5_year to another amount in the response.
 - Delete param person in the response.
 - Replace value of param person from json to xml in the response.

#### All rules settings Fiddler should be uploaded to GitHub.
