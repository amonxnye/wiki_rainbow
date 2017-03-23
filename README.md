# wiki_rainbow

How to use rainbow Demo (Beta)

/**Email**/
amonxnye@gmail.com for Activiation

/**For Users**/
Visit https://payrainbow.com/landing/
This is our Home page which will welcome users

/**For new visitors**/
Signup and follow the promonts (use either Google or Email/Password)

https://payrainbow.com/landing/signup.html ( Still under construction)

or
Recommended
https://payrainbow.com/shop_rainbow/login.html ( For Google only,/**Recommended**/)

/**Note**/ 
Please check your email for rainbow Account details
Uses Ugandan Number currently for verification of transactions
 
/**Dashboard**/
You will then forwarded to your dashboard
http://payrainbow.com/user/

There you get your balances.

/**For Demo shoping site**/

https://payrainbow.com/shop_rainbow/
This is a sample shopping site developed with the API to demo how the payment would work


/**For developers**/

This is php Curl Implementation for the API call,So in less than 25 lines, one can start an ecommerce site.

// Get cURL resource
$curl = curl_init();

// Set some options - we are passing in a useragent too here
curl_setopt_array($curl, array(
    CURLOPT_RETURNTRANSFER => 1,
    CURLOPT_URL => 'https://payrainbow.com/purchase_curl.php',
    CURLOPT_USERAGENT => 'DEMO',
    CURLOPT_POST => 1,
    CURLOPT_POSTFIELDS => array(
        'card' => 'amon',
        'amount' => '2000',
        'seller' => '2',
        'product' => 'mangoes',
        'quantity' => '100',
        'name' => 'amonte',
        'pin' => '2568',
        'key' => 'qwertyuio23456789qwertyui345678'
    )
));

// Send the request & save response to $resp
$resp = curl_exec($curl);

// Close request to clear up some resources
echo  $resp;

curl_close($curl);\

/**NOTE**/ This implememntation will not with these datails , this is just for demo.






