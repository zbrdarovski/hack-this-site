**HackThisSite**

**Basic 1**

In this basic the password was written as a comment in the HTML code. With the help of Inspect Elements (F12) we found the comment where the

![A screenshot of a computer Description automatically generated with medium confidence](./images/image1.png)

Image 1: Using Inspect Elements to discover the hidden password.

**Basic 2**

In this basic password validation script is missing. Wee entered the site by leaving the password field blank and clicking on the submit button.

![Graphical user interface, text Description automatically generated](./images/image2.png)

Image 2: Lack of script for password validation.

**Basic 3**

In this basic they have added password validation script. However, the script is visible to everyone. Using Inspect Elements we discovered where the password is saved (password.php). The script is accessible and it shows the password.

![Graphical user interface Description automatically generated](./images/image3.png)

Image 3: Checking where the password is saved.

![Graphical user interface, application, Word Description automatically generated](./images/image4.png)

Image 4: Accessing the script and retrieving the password.

**Basic 4**

In this basic a mail address was added where the password is being sent. We are able to change the email to our own. We have used Inspect Element to change the email to our own and send the password to our mailbox.

![Graphical user interface, application Description automatically generated](./images/image5.png)

Image 5: Using Inspect Elements to change the email.

![Graphical user interface, text, email Description automatically generated](./images/image6.png)

Image 6: We read the password from my mailbox.

**Basic 5**

For this basic we used FireFox Browser and followed the steps from basic 4.

![Graphical user interface, text Description automatically generated](./images/image7.png)

Image 7: We changed the email using Inspect Elements.

![Graphical user interface, text, application, email Description automatically generated](./images/image8.png)

Image 8: We read the password from my email.

**Basic 6**

In this basic the encrypted password and the algorithm used to encrypt it were publicly available. With enough persistence and time, the password can be decrypted. At the beginning, we noticed a pattern in the encryption. With the help of an ASCII table we slowly decrypted the password.

![Text Description automatically generated](./images/image9.png)

Image 9: From password A we get code B by replacing each symbol of password A with a symbol that is i - positions further away in the ASCII table from the currently selected symbol of password A.

![Graphical user interface, application, table Description automatically generated](./images/image10.png)

Image 10: ASCII table used in decoding.

![A screenshot of a computer Description automatically generated with medium confidence](./images/image11.png)

Image 11: Testing the password in encoding file.

**Basic 7**

In this basic using UNIX command pipeline we retrieved the list of files in the system. We figured out which file hides the password and accessed it through the file system and read the password.

![Graphical user interface, text Description automatically generated](./images/image12.png)

Image 12: Pipelining commands in UNIX.

![Graphical user interface, application Description automatically generated](./images/image13.png)

Image 13: From the bottom of the calendar we read the file name where the password is hidden.

![Graphical user interface, text, application Description automatically generated](./images/image14.png)

Image 14: The password is visible in the file.

**Basic 8**

Useful link: [Server-Side Includes (SSI) Injection](https://owasp.org/www-community/attacks/Server-Side_Includes_(SSI)_Injection) (available on 26.11.2024). We used SSI Injection to find the file that contains the password. We read the password from the file.

![A screenshot of a computer Description automatically generated with medium confidence](./images/image15.png)

Image 15: Retrieving the list of files using SSI Injection.

![A screenshot of a computer Description automatically generated with medium confidence](./images/image16.png)

Image 16: Retrieving the file list with SSI Injection.

![Graphical user interface, text, application, email Description automatically generated](./images/image17.png)

Image 17: Retrieving the directory name that hides the password.

![Graphical user interface, text, application Description automatically generated](./images/image18.png)

Image 18: Reading the password from the directory.

**Basic 9**

In this basic we were able to use SSI Injection to read the contents of the directory that hides the name to the password directory. Once we got the name of the password directory we traversed the directory tree to access it.

![A screenshot of a computer Description automatically generated with medium confidence](./images/image19.png)

Image 19: Absolute path of the directory that hides information about the password directory.

![A screenshot of a computer Description automatically generated with medium confidence](./images/image20.png)

Image 20: SSI Injection using absolute path.

![Graphical user interface, text, application, email Description automatically generated](./images/image21.png)

Image 21: Finding the password directory name.

![Graphical user interface, application, Word Description automatically generated](./images/image22.png)

Image 22: Reading the password.

**Basic 10**

In this basic we used JavaScript commands to check the cookie contents and to authorize login.

![Graphical user interface, text Description automatically generated](./images/image23.png)

Image 23: javascript:alert(document.cookie);

![Graphical user interface, text Description automatically generated](./images/image24.png)

Image 24: javascript:alert(document.cookie="level10_authorized=yes");

![A screenshot of a computer Description automatically generated with medium confidence](./images/image25.png)

Image 25: Once given authority, we can login with any password.

**Basic 11**

Useful link: [Hiding files with apache](https://stackoverflow.com/questions/11776369/hiding-files-with-apache) (available on 26.01.2024).

In this basic the .htaccess directory hides the password directory name. Using Inspect Elements we found out that file containing song names is hidden somewhere. All of the songs are composed by Elton John. Perhaps a directory connected to this name was hidden on the file system. Sure enough we traversed through directories that spelled out the name Elton. This is where the .htaccess directory was hidden. Inside the .htaccess we found the name of the password directory DaAnswer. Inside DaAnswer we found the password and successfully logged in the website.

![Graphical user interface, text, application, email Description automatically generated](./images/image26.png)

Image 26: Using Inspect Elements to find a hint.

![Graphical user interface, text, application Description automatically generated](./images/image27.png)

Image 27: Traversing the directory tree to find the .htaccess file location.

![Graphical user interface, text, application Description automatically generated](./images/image28.png)

Image 28: Accessing the .htaccess file.

![Graphical user interface, text, application Description automatically generated](./images/image29.png)

Image 29: Contents of the password directory.
