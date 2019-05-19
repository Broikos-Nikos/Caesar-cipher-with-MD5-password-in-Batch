# Caesar-cipher-with-MD5-password-in-Batch

Caesar cipher with MD5 password in Batch. This Batch program encrypts and deprypts a file with a password. The main use of the program is to encrypt text content.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

The batch files like this, are meant to run on Windows based systems. Also Batch are executed in the command line. Finally a safe and dedicated to the program folder is recommended.

```
Windows 7,8,10
Working CMD (No administration privileges needed - No known version requirements)
Dedicated folder directory
```

### Installing

A step by step series of examples that tell you how to get started

Download the .zip file.

Unzip the file in the preferred folder.
```
Example: "C:\preferred_folder\"
```
Use a MD5 encrypting service to encrypt a password to use. 

Create a file with the exact name "mytextx.txt" in the preferred folder.
```
Example: "C:\preferred_folder\mytextx.txt"
```
Open the "mytextx.txt" file and enter the MD5 password to the last line.


## Running the tests

A good way to validate the "mytextx.txt" file, is to enter every printable character before the last line with the MD5 password. 

The password chosen is the word "password",which corresponds to the following MD5-hash:"5f4dcc3b5aa765d61d8327deb882cf99"

"mytextx.txt" file contents example:
```
ABCDEFGHIJKLMNOPQRSTUVWXYZ
abcdefghijklmnopqrstuvwxyz
0123456789
@#-/\ .,?;:=-_+()[]{}
5f4dcc3b5aa765d61d8327deb882cf99
```

With these contents in the .txt file, run the cipher.bat file.

Enter the password:"password" when asked.

Let the program finish.

Notice there is a mytextx.encr file and the mytextx.txt file is deleted.

Re-run the cipher.bat file

Enter the password:"password" when asked.

Check the contents of the mytextx.txt file to be the same as before.

## Use

When needing to decrypt the contents of mytextx, run the cipher.bat file, enter the used password and let the program finish.

When needing to encrypt the contents of mytextx, run the cipher.bat file, enter the used password and let the program finish.

## Limitations

The program is limited by:

* The batch printable characters.
* Password length - Must not be too long or too short. Total password length varies based on each MD5 hash.
* It is breakable, but the point is to make the resources needed to decipher outweigh the reward.
* If there are more than 100 lines of text, the progress bar does not work properly. It is scheduled to be solved in a later version.

## Authors

* **Broikos Nikos** - *Programming and release* - [Broikos Nikos](https://github.com/Broikos-Nikos)

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Main inspiration from my mother, who, as an elder person, has trouble remembering passwords but also feels unsafe to store them in a simple .txt file. So this very simple encrypter/decrypter was created.
