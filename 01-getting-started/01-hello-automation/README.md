# 🚀 Welcome to Your First Bash Adventure!

Hey there, future automation wizard! Ready to start your journey into the exciting world of bash scripting? Let's create something cool together! 

## 🎯 Your Mission

Create a smart greeting script that:
- Says hello in style! 
- Knows what time of day it is
- Remembers people's names
- Adds some cool colors!

## 🎓 What You'll Learn
- How to write your first bash script
- Working with variables
- Using command-line arguments
- Adding colors to your terminal
- Making time-based decisions

## 🚀 Getting Started

### Step 1: Create Your First Script
1. Open your terminal
2. Navigate to this directory:
```bash
cd 01-hello-automation
```
3. Create your script file:
```bash
touch hello.sh
```
4. Make it executable:
```bash
chmod +x hello.sh
```

### Step 2: Basic Script Structure
Open `hello.sh` in your favorite editor and start with this:
```bash
#!/bin/bash

# Your first bash script! 
echo "Hello, World!"
```

## 🎮 Challenge Levels

### Level 1: Basic Greeting 🌱
Make a script that says "Hello, World!"
```bash
# Example output:
Hello, World!
```

### Level 2: Personal Greeting ⭐
Ask for the user's name and say hello
```bash
# Example output:
What's your name? Sarah
Hello, Sarah!
```

### Level 3: Time-Based Greeting 🌟
Add different greetings based on time:
- 5 AM - 12 PM: Good morning
- 12 PM - 6 PM: Good afternoon
- 6 PM - 5 AM: Good evening

```bash
# Example output (at 3 PM):
What's your name? Sarah
Good afternoon, Sarah!
```

### Level 4: Colorful Greeting 🌈
Add some color to your output!
```bash
# Colors you can use:
RED='\033[0;31m'
GREEN='\033[0;32m'
BLUE='\033[0;34m'
NC='\033[0m' # No Color
```

## 🔍 Testing Your Script

Run your script using:
```bash
./hello.sh
```

Or with an argument:
```bash
./hello.sh Sarah
```

## 💡 Helpful Tips

### Getting The Current Hour
```bash
current_hour=$(date +%H)
# This gives you the current hour (0-23)
```

### Reading User Input
```bash
echo "What's your name?"
read name
```

### Using Command Line Arguments
```bash
name=$1  # Gets the first argument
```

### Adding Colors
```bash
echo -e "${GREEN}Hello${NC}"  # Print in green
```

## 🎯 Success Checklist
- [ ] Script runs without errors
- [ ] Greets user by name
- [ ] Shows correct time-based greeting
- [ ] Uses colors in output
- [ ] Handles both user input and command line arguments

## 🌟 Bonus Challenges
1. Add multiple language support
2. Create a fancy ASCII art banner
3. Add different colors for different times of day
4. Add fun emoji based on time 🌅 🌞 🌙

## 🆘 Need Help?

### Common Issues and Solutions:
1. **Script not running?**
   - Check if it's executable (`chmod +x hello.sh`)
   - Make sure you're in the right directory

2. **Colors not working?**
   - Use `echo -e` to enable color interpretation

3. **Time not working?**
   - Double-check your conditions
   - Print the hour for debugging

### Still Stuck?
Check out the hints folder:
1. `hint1.md` - Basic script structure
2. `hint2.md` - Working with time
3. `hint3.md` - Adding colors

## 🎨 Example Script Structure
```bash
#!/bin/bash

# Colors
GREEN='\033[0;32m'
NC='\033[0m'

# Get the name (either from argument or user input)
if [ -z "$1" ]; then
    echo "What's your name?"
    read name
else
    name=$1
fi

# Basic greeting
echo -e "${GREEN}Hello, $name!${NC}"
```

## 🎉 Ready to Start?
1. Create your script
2. Try the basic greeting
3. Add new features one by one
4. Test everything
5. Share your creation!

Remember: Every master programmer started with their first "Hello, World!" You've got this! 💪

Happy coding! 🚀
