# 100 Days Of Code - Log

### Day 1: December 12, Thursday

**Today's Progress**: I've been working on the Roller Blinds Wifi project, investigating why does my stepper motor (BYJ48) always spin in the same direction using J5. I found that the problem is related to the sequence of the motors, J5 is using a different from the one that specify the builder, [here](http://eeshop.unl.edu/pdf/Stepper+Driver.pdf) is the documentation about it. What I tried:
- Rebuild from scrath the Stepper library using J5.Pin, but for a strange reason that I didn't have much time to see it doesn't like moving the stepper with Arduino's code.
- Create a new issue in J5's repository to see if anyone had this trouble and how I can manage to solve this problem. I looked up in the codebase of the framework but I didn't find anything related to the sequence.

**Link(s) to work**
1. [Roller Blinds Wifi](https://github.com/EmaSuriano/roller-blinds-wifi)
2. [Issue in J5](https://github.com/rwaldron/johnny-five/issues/1424)

### Day 2: December 13, Wednesday

**Today's Progress**: I've been working with Cato trying to understand J5's code of Stepper class and see how we can change the sequence of the stepper. To do this we clone J5 repo and add a simple test connection file in order to be able to debug it. Sadly, we didn't find anything ... Right now there are 2 reasonable possibilities:
1. Keep looking in the Stepper class code, there are strange variables like `this.io` that I think that has the magic inside.
2. Implement another driver (fisically) that works with 2 pin so we don't have this Direction problem anymore, to do that I have a Pololu driver but it works with 9V so we need a power supply to make it work.

**Link(s) to work**
1. [Fork J5 repo](https://github.com/EmaSuriano/johnny-five)
