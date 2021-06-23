# SCENARIO
 
When you are an owner of an industrial facility in the UK, you have a plant or factory
that produces emissions out of a chimney into the atmosphere, you are obliged by law
to record what gases or particulates those are and report it to the authorities.
This is so we can get a picture of how much pollution is emitted in different places in
the country and by what facilities, that’s required by the UK government purposes.
We also then aggregate that up and send on to the European Authorities.
 
Ricardo has a contract for gathering this information across the UK and we have a
simple portal where people can login and say here’s my facility and I’ve produced this
much emissions today and here’s my data.
 
Let’s imagine we have a web form somebody filled it in, it’s just a standard HTML form,
they’ve filled in their details and they submit their data, which is coming to us over
a POST request.
 
So we need to write a bit of PHP code to process that data and store it in the database
so we can later on analysis the total amount of Carbon Monoxide produced in, say,
Oxfordshire, so I can do some aggregate queries later on.
 
Write a simple bit of PHP, there is no need to render any output as such, it’s just to store the data.

```php
/**
 * Here's the detail of the incoming data.
 *
 * Q:  Write some code which will receive some form input and store it in a database.
 *
 * HTML Form input fields are;
 *
 *       Full Name (string)
 *       Company (string)
 *       Latitude (float)  - of the facility producing the emissions
 *       Longitude (float) - of the facility producing the emissions
 *       List of pollutants & related emission reading - Two arrays, for example; [['NO2', 'PM2.5'], [12.4, 15.6]]
 *       Date (string) - date the emission reading was taken 
 *       Time (string) - time the emission reading was taken (on an hourly basis)
 *       Comments (string) - simple comment for the whole of the hourly submission
 * 
 * All supplied in an $input array
 * 
 * Assume $db is a new PDO() object or your favourite ORM
 */
<?php
```
