<h1>the 1st script is hello.sh<h1>
code;
  
#!/bin/bash
echo "hello devops"
<h1>what I learnd</h1>
sheband is not mandatory but to use ot is best practice
  
<h1>2nd script is variables.sh</h1>
code;

#!/bin/bash

Name="Ahmar"

Role="devops enginerriner"

echo "my Name is $Name and im an aspiring $Role"

<h1>what I learnd</h1>

$ sign is very important for the script to run successfully. Otherwise the script will not ba able to use the user input.
using single or double quotes doesn't affect the script

<h1>the 3rd script is greet.sh<h1>
code;
  
read -p "enter your name" name

read -p "enter the tool" tool

echo "my name is $name and i use $tool frequently"

<h1>what I learnd</h1>

I did not  learn anything new frim this script as the usage of $ sign was clarified in the 2nd script

<h1>the 4th script (1/2) is check_number.sh <h1>
code; 
#!/bin/bash

read -p "enter a number " a

if [ $a -gt 0 ]; then
        echo "the given number is positiv"
elif [ $a -lt 0 ]; then
        echo "the given number is negative! "
elif [ $a -eq 0 ]; then
        echo "the given number is zero"
else
        echo "i have ni idea"
fi

<h1>what I learnd</h1>

I learned alot while creating this script I also used AI just to see what what issue are remaining after I used all my troubleshootimg skills.
<h1>the 4th script (2/2) is file_check.sh <h1>
code;
#!/bin/bash

if [ -f "hello.sh" ]; then
        echo "file exsits!"
else
        echo"file does not exists!"
fi
<h1>what I learnd</h1>
I learned that -f is used for file and -d for directory, -dpkg for a package. these are build-in commands
<h1>5th script is server_check.sh</h1>
code;
#!/bin/bash

read -p "enter the service name" service

read -p "do you want to check the status" status

if [ $status == y ]; then
        systemctl status $service
        echo "above is the status"
elif [ $status == n ]; then
        echo "status skipped"
fi
<h1>what I learnd</h1>
I was able to create this script with ease as I just combined the logic fron all above scripts.
