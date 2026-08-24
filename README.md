AIM
To control the speed of a DC motor using Pulse Width Modulation (PWM) with a development board.

ALGOTHRIMN
Initialize the development board and set the motor control pin as an output.
Generate a PWM signal at the required frequency.
Set an initial PWM duty cycle.
Apply the PWM signal to the DC motor through a suitable motor driver.
Vary the duty cycle to increase or decrease the motor speed.
Observe the corresponding change in motor speed.
Repeat the process for different duty-cycle values.
Aim
To control the speed of a DC motor using Pulse Width Modulation (PWM) with a development board.

Algorithm
Initialize the development board and set the motor control pin as an output.
Generate a PWM signal at the required frequency.
Set an initial PWM duty cycle.
Apply the PWM signal to the DC motor through a suitable motor driver.
Vary the duty cycle to increase or decrease the motor speed.
Observe the corresponding change in motor speed.
Repeat the process for different duty-cycle values.
Procedure
Connect the DC motor to the motor driver circuit.
Connect the motor driver to the development board.
Connect the required power supply and ensure a common ground.
Configure the motor control pin for PWM output.
Upload the PWM motor-control program to the development board.
Start the motor with a low PWM duty cycle.
Gradually increase the duty cycle and observe the increase in motor speed.
Decrease the duty cycle and observe the reduction in motor speed.
Record the motor response for different PWM values.
PROGRAM
onst int motorPin = 9;
const int potPin = A0;

void setup() {
  pinMode(motorPin, OUTPUT);
}

void loop() {
  int potValue = analogRead(potPin);
  int pwmValue = map(potValue, 0, 1023, 0, 255);
  analogWrite(motorPin, pwmValue);
Result
image image
The speed of the DC motor was successfully controlled using PWM. Increasing the PWM duty cycle increased the motor speed, while decreasing the duty cycle reduced the motor speed.
PROGRAM

RESULT
image image
The speed of the DC motor was successfully controlled using PWM. Increasing the PWM duty cycle increased the motor speed, while decreasing the duty cycle reduced the motor speed.
OUTPUT
<img width="1228" height="741" alt="WhatsApp Image 2026-08-24 at 10 45 16 AM" src="https://github.com/user-attachments/assets/06188ca4-753d-4b3c-ae0d-87da2647c2fc" />

