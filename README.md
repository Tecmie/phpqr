# phpqr
Create PNG QR code images for Emails, URLs and text from inputed text


Create a PHPQR code 
// include BarcodeQR class
include "BarcodeQR.php";

// set BarcodeQR object
$qr = new BarcodeQR();

// create URL QR code
$qr->url("www.facebook.com");


// For content
$qr->content("type", "size", "content");

// email
$qr->email("email", "subject", "message");

// geo location
$qr->geo("lat", "lon", "height");

// phone
$qr->phone("phone");

// sms
$qr->sms("phone", "text");

// text
$qr->text("text");

// URL
$qr->url("url");

// wifi connection
$qr->wifi("type", "ssid", "password");



For output QR code

// display new QR code image
$qr->draw();

// Then Save File with 
$qr->draw(120, "tmp/qr-code.png");
// This will save the qr as a square 120x120 file

