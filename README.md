# WebApplication for Event Registration

## AIM:
To create a UX design and develop a web application for event registration.

## PROGRAM:

### home.html

```
<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>Anime con!</title>
  </head>
  <body>
    <div class="jumbotron">
        <div class="cotainer">
            <h1 class="display-4">Adelaide Production Company</h1>
            <p class="lead">Welcome to the International Anime Conference!!</p>
            <hr class="my-4">
            <p>A place where all weebs and Anime fans meet. This conference is open to all around the world! All are welcome to do a cosplay</p>
            <p class="lead">
            <a class="btn btn-primary btn-lg" href="#" role="button">Learn more</a>
            </p>
        </div>
    </div>
    <div class="container">
        <div class="row">
            <div class="col-12 text-center">
                <h1>1 week International Anime conference</h1>
            </div>
        </div>
        <div class="row">
            <div class="col-12 text-center">
                <a href="/register/" class="btn btn-primary btn-lg" role="button">Register</a>
            </div>
        </div>
    </div>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js" integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
  </body>
</html>
```
### register.html

```
<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>Registration</title>
</head>

<body>
    <div class="jumbotron">
        <div class="container">
            <div class="jumbotron jumbotron-fluid" style="background-color:aquamarine;">
                <div class="container  text-center">
            <h1 class="display-4">Anime Conference</h1>
            <p class="lead">A place to meet Anime fans all around the world!</p>
            <hr class="my-4">
            <p>The participants will be exposed to the history of Animes and they will be a cosplay competition and fun prizes at the end!</p>
            <p class="lead">

            </p>
        </div>
    </div>
    <div class="container">
        <div class="row">
            <div class="col-12">
                <h1>Application</h1>
            </div>
        </div>

        <form method="POST" action="/register/">
            {% csrf_token %}


            <div class="form-group">
                <label for="name">Name</label>
                <input type="name" class="form-control" name="username" id="username" aria-describedby="emailHelp"
                    placeholder="Enter name">
            </div>
            <div class="form-group">
                <label for="phone">Phone</label>
                <input type="phone" class="form-control" name="phone" id="phone" placeholder="phone">
            </div>
            <div class="form-group">
                <label for="exampleInputEmail1">Email address</label>
                <input type="email" class="form-control" name="exampleInputEmail1" id="exampleInputEmail1"
                    aria-describedby="emailHelp" placeholder="Enter email">
                <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone
                    else.</small>
            </div>
            <div class="form-group">
                <label for="institutionname">Institution name</label>
                <input type="institutionname" class="form-control" name="institutionname" name="institutionname"
                    id="institutionname" placeholder="institutionname">
            </div>
            <button type="submit" class="btn btn-primary">Submit</button>
        </form>

    </div>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
        integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
        integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
        crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
        crossorigin="anonymous"></script>
</body>

</html>
```

### success.html
```
<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>YAAY!</title>
  </head>
  <body>
    <h1>CONGRATSS!! YOU APPLICATION HAS BEEN ACCEPTED!!</h1>
    <h2>now you are also a part of stacy's
    </h2>
    <a href="/home/" class="btn btn-primary btn-lg active" role="button" aria-pressed="true">Home</a>
    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js" integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
  </body>
</html>
```

### failed.html
```
<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>SORRY :(</title>
  </head>
  <body>
    <h1> THE SEATS ARE FILLED!!</h1>
    <h2> thank you for participating...
    </h2>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js" integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
  </body>
</html>
```

### listofparticipants.html

```
<!doctype html>
<html lang="en">

<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
        integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">

    <title>International Anime conference</title>
</head>

<body>
     <div class="jumbotron" style="box-sizing: border-box;">
      <div class="p-5 text-center bg-image" style="
      background-image: url('https://dubeat.com/wp-content/uploads/cultural-fests.jpg');
      height: 200%;background-repeat: no-repeat;background-size: cover;">
        <div class="container">
      
      
        <div class="container  text-center">
            <h1>Adelaide production company</h1>
            <h1 class="display-4">Hello, Guys!</h1>
            <h1 class="display-4">Welcome to our International Anime Conference</h1>
        </div>
      </div>
            
        <div class="row">
            <div class="col-12">
                <h1>Congragulations!</h1>
            </div>
        </div>
        <div class="row">
            <div class="col-12">
                <table class="table">
                    <thead>
                        <tr>
                            <th scope="col">NAME</th>
                            <th scope="col">EMAIL</th>
                            <th scope="col">PHONE</th>
                           
                        </tr>
                    </thead>
                    <tbody>

                        <tr>
                            <td>kesha</td>
                            <td>keshaa@gmail.com</td>
                            <td>234242</td>
                            
                        </tr>

                        <tr>
                            <td>max</td>
                            <td>max@gmail.com</td>
                            <td>9876234242</td>
                            
                        </tr>

                        <tr>
                            <td>sabrina</td>
                            <td>sabrina@gmail.com</td>
                            <td>9987764123</td>
                            
                        </tr>

                        <tr>
                            <td>olivia</td>
                            <td>olivia@gmail.com</td>
                            <td>9988734234</td>
                            
                        </tr>

                        <tr>
                            <td>Samantha</td>
                            <td>samantha@gmail.com</td>
                            <td>6722337234</td>
                            
                        </tr>

                        <tr>
                            <td>Debra</td>
                            <td>debra@gmail.com</td>
                            <td>9088654456</td>
                            
                        </tr>

                        <tr>
                            <td>Vierne</td>
                            <td>vierne@gmail.com</td>
                            <td>7885366336</td>
                            
                        </tr>

                        <tr>
                         <td>Mellisa</td>
                            <td>mellisa@gmail.com</td>
                            <td>7888966336</td>  
                            
                        </tr>

                        <tr>
                         <td>Lisa</td>
                            <td>lisa@gmail.com</td>
                            <td>9985366336</td>
                        </tr>

                        <tr>
                           <td>kelly</td>
                            <td>kellyo@gmail.com</td>
                            <td>7886739336</td>
                        </tr>

                        <tr>
                           <td>kendra</td>
                            <td>kendra@gmail.com</td>
                            <td>788537886</td>
                        </tr>

                        <tr>
                            <td>pierson</td>
                            <td>pierson@gmail.com</td>
                            <td>8977566336</td>
                        </tr>

                        <tr>
                            <td>Sophie</td>
                            <td>sophie@gmail.com</td>
                            <td>9888766336</td>
                        </tr>

                        <tr>
                            <td>Jules</td>
                            <td>jules@gmail.com</td>
                            <td>9087533232</td>
                        </tr>

                    </tbody>
                </table>
            </div>
        </div>
        <div class="row">
            <div class="col-12 text-center">
                <a href="/home/" class="btn btn-primary btn-lg" role="button">Home</a>
            </div>
        </div>
    </div>

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
        integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
        crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
        integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
        crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
        integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
        crossorigin="anonymous"></script>
</body>

</html>
```

## OUTPUT:

![output](./static/img/oo1.jpg)

![output](./static/img/ooo2.jpg)

![output](./static/img/ooo4.jpg)

![output](./static/img/ooo5.jpg)


## RESULT:
Thus a website is designed for the manufacturing company and is hosted in the URL http://aishree.student.saveetha.in:8000/.
