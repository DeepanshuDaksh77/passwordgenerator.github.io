<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Python password generator</title>
    
    <link rel="stylesheet" href="https://pyscript.net/alpha/pyscript.css" />
    <script defer src="https://pyscript.net/alpha/pyscript.js"></script> 
    <style>
    body{
        background-color: lightcoral;
        text-align: center;
        font-family: Arial, Helvetica, sans-serif;
        font-size: large;
    }
    
    </style>

</head>
<body>
    <h1><b>Pyscript Test</b></h1>
    <py-script>

        import string
        import random

        if __name__ == '__main__':
            s1 = string.ascii_lowercase
            s2 = string.ascii_uppercase
            s3 = string.digits
            s4 = string.punctuation
            pl = int(input("Enter password length:\n"))

            s = []
            s.extend(list(s1))
            s.extend(list(s2))
            s.extend(list(s3))
            s.extend(list(s4))

            random.shuffle(s)
            print("Your password is:","".join(s[0:pl]))

    </py-script>
</body>
</html>
