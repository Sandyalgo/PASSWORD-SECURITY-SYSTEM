ABSTRACT:

    4-bit password security system (using NOR & XOR gates)
    The project is a security system which allows only authorized access to users
    with a password. This system provides a user friendly security system for
    organizations and homes.
    
    The idea of this system is that the 4 switches "KEY CODE SWITCHES" acts as
    holding the correct password for unlocking the lock. On the other hand the
    other 4 switches "DATA ENTRY SWITCHES acts as data entry point where the
    code is to be entered to open lock. The "KEY CODE SWITCHES" have static
    value and is hidden from the person who is trying to open the lock. If the
    "DATA ENTRY CODE matches the "KEY CODE" then the green LED will light up
    and the lock will open. While if the "DATA ENTRY CODE" does not match the
    "KEY CODE" then the red LED will glow which is an alarming situation that
    some wrong person is unlocking the lock.
    
    The project offers valuable hands-on experience in digital logic design,
    providing a practical understanding of how digital circuits can be used
    to create secure systems. Students gain skills in circuit design,
    implementation, and debugging, reinforcing theoretical knowledge
    with practical application.
    
LIST OF COMPONENTS

    	7408 quad AND gate.
    	7486 quad XOR gate.
    	Two, eight / four-position DIP switches.
    	Two light-emitting diodes.
    	7404 Four NOT gate.
    	Pushbutton switch, normally open.
    	9-volt battery. 

WORKING

•	Setting the Key Code

    o	The key code is set using the first set of 4-position DIP switches (SW1-SW4). This key code represents the correct password that grants access. 
        The key code is static and hidden from the user attempting to gain access.
        
•	Entering the Password

    o	The user enters a password using the second set of 4-position DIP switches (SW5-SW8). This entered password is the data that will be compared against the key code.
    
•	Comparison Using XOR Gates

    o	Each bit of the entered password is compared with the corresponding bit of the key code using the XOR gates in the 7486 IC. The XOR gate outputs a high signal (1) 
        if the bits are different and a low signal (0) if the bits are the same.
    o	If the entered password matches the key code exactly, all XOR gate outputs will be low (0).
    
•	Logic Processing with AND and NOT Gates

    o	The outputs of the XOR gates are fed into a combination of AND and NOT gates. These gates process the XOR outputs to produce a single output that 
        determines whether the entered password matches the key code.
    o	If all XOR gate outputs are low (indicating a match), the final processed output will be configured to light up the green LED.
    o	If any XOR gate output is high (indicating a mismatch), the final processed output will be configured to light up the red LED.
    
•	Indicating the Result

    o	Green LED (Correct Password): When the entered password matches the key code, the processed output activates the green LED, indicating successful access.
    o	Red LED (Incorrect Password): When the entered password does not match the key code, the processed output activates the red LED, signaling unauthorized access.
    
•	Pushbutton Switch Activation

    o	The pushbutton switch is used to initiate the password comparison process. When the button is pressed, it allows the current to flow through the circuit, 
        enabling the comparison logic to operate.
        
•	Power Supply

    o	The entire circuit is powered by a 6-volt battery. Proper connections ensure that each component receives the necessary voltage to function correctly.

RESULTS AND OUTPUT


![Circuit Connections](https://github.com/user-attachments/assets/d792aa92-be2e-4402-93de-5c5f95c1f170)

REFERENCES

https://circuitverse.org/users/245991/projects/password-security-system-0b152a3d-a8a8-4676-8546-1f0d3b9d3b18

