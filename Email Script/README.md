# PHP Email Scrip

This will be a simple PHP script to send an email based on a POST from a form. We will make 2 versions of this
* one using a PHP POST in an HTML From
* Another using a React Component and JS helper function to POST the output of the form

Between these 2 front ends the slight differences in handling POST input should be made clear to help better understand the basic PHP logic needed when dealing with email and serve to create a start scrip most can use to add this to any site they work on.

## Step 1 | What do we need to do?
The first step in any programming is to think out the logic. I have the best heard this explained with the truism of 2 weeks of coding can save you 20 min of planing. So keeping this in mind, what does out code need to do?

```
1) We need to get the info we will email
2) we need to send that info somewhere we can do something with it
3) we need to take that info and make sure it is in a format we need to do something with
4) we need to assemble that info into an email
5) we need to send that email where it should go
```

## Step 2 | Code "1) We need to get the info we will email"

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

#### Understanding our <input />
The 3 values here are the minim to have a usable form. So let us take a sec to understand them.

```
type="text"
```
This is just like it sounds, what the type of this form filed or```input``` is. As is always a good practice if you are unsure what ```type``` you need to use you can check the [documentation] (https://www.w3schools.com/html/html_form_input_types.asp).

```
name="name_value"
```
This one is strait forward but I will point out a foobar no-foobar I see some more new or Jr Dev strugle with. In our sample code ```form.html``` this line is ```name="name"```......




Overall any code is this simple, you just need to make sure you have all the steps, and then code each step. Not necessarily in order.




##### IN PROGRESS, pushing up in my free time....
