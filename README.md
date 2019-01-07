# MpesaDaraja
This is an accompanying repository for a blog that gives a step by step on how to implement successfully the Safaricom *Daraja API*,It is a very simple application that you can use as a launching pad to build out your android application that implements the *MPESA API*.
It implements the LNMO api in sandbox mode but it should be relatively easy to move to production with this, but you will have to remove some loggers for security purposes.

### So Where is the blog?
So the blog i divided into two parts. THe first part is a basic introduction to those who have yet to interact with the Safaricom Daraja API. In this first part you learn how to create a project, get Consumer Keys and Consumer Secrets and Start you LNMO app.

The second part will be showing how to plug these values into your android application to get it to make transactions.

##### Part 1
[Mpesa Integration](http://overflow.moringaschool.com/engineering/mpesa-integration-in-android-applications.html)

## Backend (CallBack)
In order for your transactions to complete successfully, you need to provide a Callback Url which will receive all communication on failure or passing of
your requests.

The following is a [link](https://gist.github.com/lawrence254/39313589b32f2b9a399d4b49f0e3e9ea) to the callback back files I'm using. 
You only need to fill in your db username, password, host and select the db to use, create teh table to store your data and you're all set.

As a bonus, if you would like to search throught the stored data, [this](https://gist.github.com/lawrence254/48ddd8012d5b0a23481ef6b71cc18ad7) file provides a basic search 
functionality that allows you to search through your table based on the users phone number.
