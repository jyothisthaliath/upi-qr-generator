# QR Code Generator for UPI Payments

*By Jyothis Thaliath — Originally published 2017*

---

Nowadays UPI is being used as a payment alternative in many places like retail stores. But many small scale retailers are not having the expertise to generate/print QR code with their payment details. So I decided to create an app to do just that.

**QR Code Generator for UPI** is useful for retailers who wish to accept payments through UPI. The retailer can have this application installed either in a computer or smartphone.

## The Workflow

1. Retailer enters the payment information like **Name**, **Virtual Address**, **Bill Amount** and **Notes** in the app
2. Retailer generates QR code using the app
3. Customer opens any bank's UPI application in their mobile
4. Customer invokes **'Scan to Pay'** option and scans the QR code
5. Payment details of the retailer will be pre-filled in the UPI application and the customer can complete the transaction with PIN authentication
6. Retailer receives SMS about credit of amount

> In case the retailer wishes to display his payment information permanently as a **poster** in the store, they can do so by following the same procedure, leaving the "Amount" field blank. When the customer scans this code, they can input the amount manually.

## Prerequisites

- Both parties must have UPI enabled in their bank accounts
- Retailer should know his **Virtual Address (VPA)**
- Customer should have at least one UPI application in their mobile (any bank)
- Internet connectivity for both parties

## Available Channels

The app was made available in three channels:

### 1. Web App
Web application designed to run from any web browser. Open the URL in the browser, enter the details and click Generate. QR code will be displayed in a new window.

### 2. Android App
Download and install the application. Open the app, feed the required information and click generate. QR code will be opened in the browser window.

### 3. Windows Application
Workflow is same as the web application. No other requisites for running the app.

---

## The Back Story

An email from AppsGeyser reminded me of something I had created long back and totally forgotten.

In 2016, shortly after the **demonetization**, many retailers adopted SBI Buddy and Paytm to attract cashless payments. But both of these services required that the payer have a prepaid wallet account with their respective providers.

But with the advent of **UPI**, all of that was going to be changed. UPI was the game changer in payments, which allowed people to make payments out of their own bank accounts without keeping any third-party wallets.

But in the initial stages, it was all based on entering the VPA of the beneficiary provided by the bank — and didn't involve any code scans like how SBI Buddy and Paytm were doing it since the beginning.

**I saw an opportunity to bridge this gap** by providing an easy way — an app to generate UPI payment QR codes.

To start with this, I referred to the **UPI deeplink specifications** which were publicly available from NPCI to understand the request format compatible with UPI mobile applications. I used the **Google Charts API** for the generation of QR codes.

The whole app was made in **HTML5 and Javascript** — which was no easy feat for me with no web development background. It took me days to just fix the responsive design *(dynamic changes to the appearance of a website, depending on the screen size and orientation of the device being used to view it)*. But with StackOverflow and persistence, everything was possible!

I used HTML5 to build it so that I could use the same website for mobile and PC. But I knew that the app didn't stand a chance if it wasn't available as a native mobile app. That was a major challenge as I had zero knowledge of developing mobile apps. Fortunately, **AppsGeyser** came to my rescue, allowing me to package my web application into an APK that could run on any Android phone.

I had no intention to monetize the app as it was the need of the hour to help struggling retailers.

---

## The Impact

The app was well received among my colleagues at the bank. Now in the present age it is pretty outdated — most payment apps themselves carry this feature to generate and share QR codes as required.

But for me it was truly rewarding for all the hours I had put in to create something which **became useful for the masses**.

I still remember the time when the branch manager of one of the biggest branches in our region called me to convey the feedback from a businessman who was one of their prime customers. That was really a moment which I still cherish.

---

## Acknowledgements

Big thanks to **Rojish Roy** for helping me out with the venture and hosting my app on his domain (`upiguide.com` — which is no longer available).

Thanks for reading!
