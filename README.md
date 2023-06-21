# Case-Study-Global-Command-Centre-
One pager submission for AB InBev
This contains code implementation for part 2.

Problem Statement: 

To develop a notification feature that sends periodic updates to a user's Gmail account regarding their unread notifications and messages from their LinkedIn profile. The notifications are to be sent every 3 hours and should include the following information in the email body.​

Approaches:

-We install necessary dependencies and libraries: Use apt-get and pip commands to install chromium-browser, chromedriver, selenium, and openpyxl for web scraping and Excel interaction.​

-We use the webdriver from Selenium to automate the login process to LinkedIn. We provide the username and decrypted password to log in securely. ​

-We utilize the Selenium driver to navigate to the LinkedIn profile and extract the count of unread messages and notifications.​

-We load an existing Excel file, add a new row with the current timestamp and the retrieved counts of unread messages and notifications.​

-We compose an email using the smtplib library, including the number of unread messages and notifications, along with a comparison result.​

Steps:

1. Set the LinkedIn login credentials. Called the function, login_to_linkedin, to perform the login process on LinkedIn using Selenium.​

2. Defined a function, decrypt_password(), to decrypt the encrypted password.​

3. Defined a function, get_unread_data(), to retrieve the number of unread messages and notifications from the LinkedIn profile using the provided Selenium driver.​

4. Defined a function, save_data_to_excel(), to save the retrieved data to an Excel file. Defined a function, send_email_notification(), to send an email notification with the retrieved data.​

5. Closed the browser by calling selenium driver.quit()​

Conclusion:
   
Users will receive regular email notifications every three hours with the number of unread messages and notifications from their LinkedIn profiles. The email body will also include a comparison between the current data and previous occurrences.

​


