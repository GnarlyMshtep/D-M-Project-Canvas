# D-M-Project-Canvas
This is Dang & Matans' Canavas project!
Let's inspire the children :D
Njoy,
us. 
# D-M-Project-Canvas
Last updated: 7/17/2020 10:37am

*Sonars use 2 pins (trig and echo) to "capture" soundwaves. In a nutshell, these 2 pins work in tandem to allow for echolocation. There are 2 types of measurements: time sound is detected and distance. For both horizontal and vertical, there will be variables called duration_vertical/horizontal_sonar which contains the time. Don't worry about using it, just make sure to have it because time is necessary to calculate distance
Attached sonars:
    vertical - 
        trig pin variable name = trigPin_vertical, port 13
        echo pin variable name = echoPin_vertical, port 15
        function name = vertical_sonar()
        vertical measurement variable name = distance_vertical_sonar
    horizontal - 
        trig pin variable name = trigPin_horizontal, port 1
        echo pin variable name = echoPin_horizontal, port 3
        function name = horizontal_sonar()
        horizontal measurement variable name = distance_horizontal_sonar
    *IMPORTANT: call function name to begin measurements. REMEMBER: if measurement decreases, object is moving towards sonar and if measurement increases, object is moving away from sonar. 

*Servo is attached to a different Arduino board (Arduino Uno) and Uno will recieve data from ESP8266 Nodemcu regarding what mode to set servo to (off or on canvas)
Attached servo:
    marker servo - 
        servo variable name = servo, port 10
    *Just digitalWrite(servo, HIGH/LOW) to switch servo mode

Attached motors:
    lower motor (up-and-down) -
        move down variable name = lower_rotation_1, port 5
        move up variable name = lower_rotation_2, port 4
    higher motor (left-and_right) -
        move left variable name = higher_rotation_1, port 12 
        move right variable name = higher_rotation_2, port 14

Canvas Information:
    Horizontal Range (cm): [2, 10] length = 8;
    Vertical Range (cm): [5, 12] length = 7;
    Make sure sonar functions are always running (at least Make sure they occur before moving)
    To retrieve sonar measurements, string their distance variables Ex: client.println("<p>Horizontal Reading: " + String(distance_horizontal_sonar) + "</p>");

NOTE: Variables stated above have only two states (HIGH/LOW)


