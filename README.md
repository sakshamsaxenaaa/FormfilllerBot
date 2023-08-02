# FormfilllerBot
What is this FormFiller Bot,how this actually works?
# DESCRIPTION.
**Auto Form Filler Bot**

This is a Java program that utilizes Selenium WebDriver to automate the process of filling out a web form on the Dreamit website. The bot opens a Chrome browser window, navigates to the specified URL, and then fills in various fields with predefined information. Below is a step-by-step description of what the bot does:

1. Import required libraries: The program imports necessary libraries from Selenium and Java to interact with the browser.

2. Set Chrome driver path: The bot sets the path of the ChromeDriver executable on the local machine. This is required to launch the Chrome browser.

3. Create a new ChromeDriver instance: The bot creates a new instance of the ChromeDriver, which will be used to interact with the Chrome browser.

4. Maximize the window: The bot maximizes the browser window to ensure that the elements on the page are clearly visible and accessible.

5. Navigate to the URL: The bot navigates to the specified URL, which in this case is "https://www.dreamit.com/getstarted".

6. Wait for page load: The bot waits for 5 seconds to ensure that the page has loaded completely before attempting to interact with the elements. This is done using the TimeUnit.sleep() method.

7. Fill the form fields: The bot finds various input fields on the page using their XPath expressions and enters the provided information in each field. The fields filled are:
   - Email Address
   - First Name
   - Last Name
   - Phone Number
   - Country
   - State
   - City
   - Zip Code
   - Address

8. Select options from dropdowns: The bot interacts with the "Country" and "State" dropdown menus using the Select class from Selenium and selects the specified options.

9. Click the submit button: Once all the required fields are filled, the bot finds the submit button and clicks it to submit the form.

10. Close the browser: After submitting the form, the browser window is closed using the driver.quit() method to clean up the resources.

**Note**: Before running the code, make sure to update the "webdriver.chrome.driver" property with the correct path to the ChromeDriver executable on your local machine. Additionally, replace the placeholder values such as "your_email_address", "your_first_name", etc., with the actual information you want to fill in the form.

This code can be used as a starting point to automate form filling tasks on websites and can be further customized as per specific requirements. Make sure to comply with the website's terms of use and policies while using automated bots.
