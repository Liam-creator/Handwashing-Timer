/*

#include <Wire.h>
#include <LiquidCrystal_I2C.h>

LiquidCrystal_I2C lcd(0x27, 16, 2);

void setup() {

  lcd.init();
  lcd.noBacklight();
  pinMode(8, INPUT);

}

void loop() {

  int detect = digitalRead(8);

  if (detect == LOW) {

    lcd.backlight();
    lcd.display();
    lcd.clear();
    lcd.print("Hand Detected");
    lcd.setCursor(0, 1);
    lcd.print("Main Détectée");
    delay(1000);

    for (int i = 20; i > 0; i--) {

      lcd.clear();
      lcd.setCursor(0, 0);
      lcd.print("Time left:");
      lcd.setCursor(11, 0);
      lcd.print(i);
      lcd.setCursor(0, 1);
      lcd.print("Temps restes:");
      lcd.setCursor(14, 1);
      lcd.print(i);

      delay(1000);

    }

    for (int x = 0; x <= 2; x++) {
      lcd.clear();
      lcd.setCursor(0, 0);
      lcd.print("DONE!!!");
      lcd.setCursor(8, 1);
      lcd.print("FINIS!!!");
      delay(500);
      lcd.clear();
      delay(500);
    }

  }

  else {

    lcd.noBacklight();
    lcd.noDisplay();

  }

  delay(100);

} */ 
