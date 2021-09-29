# auth_jwt
Sample Inputs and expeted Outputs

http://localhost:8000/api/register
>>>>INPUT>>>> 

{
"name": "Priya",
"email": "a@a.com",
"password": "a"
}                                                                                                                                                                                                                                                                                                      >>>>OUTPUT>>>>

HTTP 200 OK
Allow: POST, OPTIONS
Content-Type: application/json
Vary: Accept

{
    "id": 9,
    "name": "mani",
    "email": "man@a.com"

}

*************************************************************************************************
http://localhost:8000/api/login
>>>>INPUT>>>>   

{
"email": "man@a.com",
"password": "ma"
}                                  
                                                                                                                                                >>>>OUTPUT>>>>
HTTP 200 OK
Allow: POST, OPTIONS
Content-Type: application/json
Vary: Accept

{
    "Logged in successfully with jwt": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpZCI6OSwiZXhwIjoxNjMyOTM3NTI4LCJpYXQiOjE2MzI5MzcyMjh9.bNG-lUq_-AA3EEU3mGfRaxjmiEjAbnPGckjbxioTyKw"
}
*************************************************************************************************

http://localhost:8000/api/login

>>>>INPUT>>>>  

{
"email": "man@a.com",
"password": "ma"
}                                  
                                                                                                                                                >>>>OUTPUT>>>>

                                                                                                                                                HTTP 200 OK
Allow: POST, OPTIONS
Content-Type: application/json
Vary: Accept

{
    "message": "successfully Logged Out"
}
