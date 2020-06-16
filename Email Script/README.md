# PHP Email Scrip

This will be a simple PHP script to send an email based on a POST from a form. We will make 2 versions of this
* one using a PHP POST in an HTML From
* Another using a React Component and JS helper function to POST the output of the form

Between these 2 front ends the slight differences in handling POST input should be made clear to help better understand the basic PHP logic needed when dealing with email and serve to create a start scrip most can use to add this to any site they work on.

## Step 1 | What do we need to do?
The first step in any programming is to think out the logic. I have the best heard this explained with the truism of 2 weeks of coding can save you 20 min of planing. So keeping this in mind, what does out code need to do?

```
//We need to get the info we will email
//we need to send that info somewhere we can do something with it
//we need to take that info and make sure it is in a form we need to do something with
//we need to assemble that info into an email
//we need to send that email where it should go
```

## Step 2 | Code our step "get the info we will email"

We will do this with a form. This how you get almost anything when it comes to the web. The simple way to do this is with a HTML and PHP form. But that is not as ideal these days as it was. It comes down to what stack you are dealing with. For this reason I will also cover how to get React to talk to our PHP. The logic of those 2 ways is just different enough that it gives you a good foundation for this PHP.

You can find the full source for the PHP form in ```form.php```. I am going to limit to the ```<form></form>``` its self here.






Overall any code is this simple, you just need to make sure you have all the steps, and then code each step. Not necessarily in order.




##### IN PROGRESS, pushing up in my free time....