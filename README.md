# CMSeeK – CMS Detection and Exploitation Tool

A content management system (CMS) is an application that is used to manage web content, providing multiple givers to create, edit and publish. Content in a CMS is typically saved in a database and displayed in a presentation layer based on a set of templates. 

In the Security World, this CMS application can contain vulnerabilities that can compromise the website on which respected CMS is working. The antiquated version of CMS can also be the path of cyber attacks on the target domain. So while performing a security audit on the victim domain, CMS Detection and version detection is done. CMSeeK tool is an automated tool developed in the Python Language. CMSeeK tool is capable of scanning numerous content management systems including WordPress, Joomla, Drupal, etc. CMSeeK tool allows you to run both simple CMS detection and deep scans, as well as multi-site scans. CMSeeK tool supports Interactive Mode and Command Line Mode for its usage.
Features of CMSeeK Tool:

  - It supports more than 150 CMS for testing or detection.
  - It is open-source and free to use.
  - It has support to the interactive mode for its usage.
  - It supports brute-forcing of CMS detection on the target domain.
  - It supports testing on multiple domains parallelly.

Detection Methods:

  - Through HTTP Headers.
  - Through Generator meta tag.
  - Through Page source code.
  - Through robots.txt file on the server.

Note: Make Sure You have Python Installed on your System, as this is a python-based tool. Click to check the Installation process:  Python Installation Steps on Linux
Installation of CMSeeK Tool on Kali Linux OS:

Step 1: Use the following command to install the tool in your Kali Linux operating system.

    git clone https://github.com/Tuhinshubhra/CMSeeK
https://media.geeksforgeeks.org/wp-content/uploads/20210901225439/Step1.jpg
Step 2: Now use the following command to move into the directory of the tool. You have to move in the directory in order to run the tool.

    cd CMSeeK

Step 3: You are in the directory of the CMSeeK. Now you have to install a dependency of the CMSeeK using the following command.

    sudo pip3 install -r requirements.txt

Step 4: All the dependencies have been installed in your Kali Linux operating system. Now use the following command to run the tool and check the help section.

    python3 cmseek.py -h

Working with CMSeeK Tool on Kali Linux OS:

Interactive Mode :

▶️ Example 1: CMS detection and Deep scan 
    
    Select Option 1
 In this example, We will be using the interactive mode for CMS detection and Deep scan on geeksforgeeks.org

▶️ Example 2: Bruteforce CMSs
  
    Select Option 3
 In this example, We will be only brute-forcing single CMS on geeksforgeeks.org

Command Mode:

▶️ Example 1: Scan Domain geeksforgeeks.or

    python3 cmseek.py -u  geeksforgeeks.org
 In this example, We will be performing CMS Detection on geeksforgeeks.org. We have specified the target in the -u tag.

▶️ Example 2: Enabling verbose output while scanning geeksforgeeks.org

    python3 cmseek.py -v -u  geeksforgeeks.org
 In this example, We will be displaying the results in a more readable way or in a verbose way. We have used -v tag for verbose mode.

