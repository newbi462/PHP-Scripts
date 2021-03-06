# PHP Email Scrip

This will be a simple PHP script to send an email based on a POST from a form. We will make 2 versions of this
* one using a PHP POST in an HTML From
* Another using a React Component and JS helper function to POST the output of the form

Between these 2 front ends the slight differences in handling POST input should be made clear to help better understand the basic PHP logic needed when dealing with email and serve to create a start scrip most can use to add this to any site they work on.

## Step 0 | What do we need to do?
The first step in any programming is to think out the logic. I have the best heard this explained with the truism of 2 weeks of coding can save you 20 min of planing. So keeping this in mind, what does out code need to do?

```
1) We need to get the info we will email
2) we need to send that info somewhere we can do something with it
3) we need to take that info and make sure it is in a format we need to do something with
4) we need to assemble that info into an email
5) we need to send that email where it should go
```

## Step 1 | Code "1) We need to get the info we will email"

We will do this with a form. This how you get almost anything when it comes to the web. The simple way to do this is with an HTML form. But that is not as ideal these days as it was. It comes down to what stack you are dealing with. For this reason, I will also cover how to get React and other JS to talk to our PHP. The logic of those 2 ways is just different enough that it gives you a good foundation for this PHP. In particular how to handle the shape of the incoming data.

You can find the full source for the HTML form in ```form.html```. I am going to limit to the ```<form></form>``` tag here.

#### Form 101
Here are the basics for a form to send an email, or really any input to any back end such as a database.
```
<form method="post" action="PHPScript.php">
  <input
    type="text"
    name="name_value"
    placeholder="What will be in the box"
  />
</form>
```

As stated from the Front-End side this is collecting the ```input``` to ```POST``` to somewhere. In this case, the target or ```action``` is going to be ```PHPScript.php``` which we will code in a moment with the logic for the Back-End side of actually sending the email. But as stated that target could be anything and do anything with the data we are going to send it.

#### Understand CRUD
We are using ```method="post"``` to send the data in this form to the ```action="PHPScript.php"``` in this case it would be the ```C``` or ```Create``` of CRUD. While beyond the scope of this tutorial you may want to take the time to look up what CRUD is and understand why and when you would use GET, POST, PUT, and DEL.

#### Understanding our ```<input />```
The 3 values here are the minim to have a usable form. So let us take a sec to understand them.

```
type="text"
```
This is just like it sounds, what the type of this form filed or```input``` is. As is always a good practice if you are unsure what ```type``` you need to use you can check the [documentation] (https://www.w3schools.com/html/html_form_input_types.asp).

```
name="name_value"
```
This one is straight forward but I will point out a foobar no-foobar I see some who are newer or Jr Dev struggle with. In our sample code ```form.html``` this line is ```name="name"```. The left side ```name=``` is a reserved value and how you tell the form input what its unique identifier is, while the right side ```="name"``` or ```="name_value"``` or ```="fooBar"``` is defined by you. This right-side value is how you tell other code what value to work with and do things with. If you want to understand this concept more lookup ```parameters``` and ```variables``` as they pertain to code.

```
placeholder="What will be in the box"
```
The ```placeholder```  is being used in place of a ```label```, while you do not strictly need a placeholder value, it has become more common to pre-fill in forms with these values that tell the user what should go there. Overall it just creates a more clean UI/UX. Like with ```name``` in our ```form.html``` this line is ```placeholder="Name"``` and it is common practice to have the placeholder, name, and so on all match.


## STEP 2 | CODE "2) we need to send that info somewhere we can do something with it"
Congratulations, this is already done for the HTML form.

Remember ```<form method="post" action="PHPScript.php">``` posts/send the info to the ```PHPScript.php``` when you click Submit.


## STEP 3 | CODE "3) we need to take that info and make sure it is in a format we need to do something with"
This step can be broken into many steps, and some of the code we will do here is overall not needed, but a best practice. This is also the step where the 2 inputs (HTML and JS/React) we are doing will be most different.

At this point we have POSTed the data, so the PHP file has it, but it has not officially put the data from the form anywhere. So some sub-steps are:
```
3a) verify the data was POSTed
3b) set that data to something we can use in our PHP
3c) move on t0 the next step...
```



## STEP 4 | CODE "4) we need to assemble that info into an email"


## STEP 5 | CODE "5) we need to send that email where it should go"





Overall any code is this simple, you just need to make sure you have all the steps, and then code each step. Not necessarily in order.




##### IN PROGRESS, pushing up in my free time....
