# Shamir-s_algorithm
1.Fisrt step to run the code in vs code make sure you the server is running.
2.You get this:
Server is running on http://localhost:3000
3.Set Up the POST Request in Postman
Open Postman.
Set Request Type to POST.
Enter URL: http://localhost:3000/calculateSecretCode

4.Add JSON Body
   Go to the Body tab.
  Select raw and then JSON from the dropdown.
  Enter the JSON data you want to send to the server
Ex:
{
    "keys": {
        "n": 4,
        "k": 3
    },
    "1": {
        "base": "10",
        "value": "4"
    },
    "2": {
        "base": "2",
        "value": "111"
    },
    "3": {
        "base": "10",
        "value": "12"
    },
    "6": {
        "base": "4",
        "value": "213"
    }
}

5.Send the Request
Click the Send button
6.If everything is working, you should see a response from your server in the Body section of the Postman response area

Output:
{
    "constantTerm": "9"
}
