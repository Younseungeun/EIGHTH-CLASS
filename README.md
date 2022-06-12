# EIGHTH-CLASS

## TOPIC
- make a code of RC car
- four-wheel drive
- 4 directions

### four-wheel drive CODE
1. int motor1PinA  = 2 ;
2. int motor1PinB =3 ;
3. int enablelPin=  11 ; //left  
4. int motor2PinA  = 4 ;
5. int motor2PinB =5;
6. int enableRPin=  10 ; //RIGHT
7. void setup() {
8. pinMode(motor1PinA, OUTPUT);     
9. pinMode(motor1PinB, OUTPUT);
10. pinMode(enablelPin, OUTPUT);
11. pinMode(motor2PinA, OUTPUT);     
12. pinMode(motor2PinB, OUTPUT);
13. pinMode(enableRPin, OUTPUT)
14. analogWrite(enablelPin, 255);//set the speed of the motor (255 is the maximum)
15. analogWrite(enableRPin, 255);
16. }
17. void loop() {                                          
18. digitalWrite(motor1PinA, HIGH);                                                                                                     
19. digitalWrite(motor1PinB, LOW);  
20. digitalWrite(motor2PinA, HIGH);                                                                                                     
21. digitalWrite(motor2PinB, LOW);                                                                                                                                 22.delay(1000);                                                                                                                                                          23. }                         
### 4 directions CODE
1. int motor1PinA  = 2 ;
2. int motor1PinB =3 ;
3. int enablelPin=  11 ; //left
4. int motor2PinA  = 4 ;
5. int motor2PinB =5;
6. int enableRPin=  10 ; //RIGHT
7. void setup() {
8. pinMode(motor1PinA, OUTPUT);     
9. pinMode(motor1PinB, OUTPUT);
10. pinMode(enablelPin, OUTPUT);
11. pinMode(motor2PinA, OUTPUT);     
12. pinMode(motor2PinB, OUTPUT);
13. pinMode(enableRPin, OUTPUT);
14. analogWrite(enablelPin, 100);//모터속도를 정해준다
15. analogWrite(enableRPin, 100);//모터속도를 정해준다
16. delay(1000);          
17. }
18. void loop() {     
19. digitalWrite(motor1PinA, HIGH);              //FRONT                                                                                    
20. digitalWrite(motor1PinB, LOW);  
21. digitalWrite(motor2PinA, HIGH);                                                                                                     
22. digitalWrite(motor2PinB, LOW);                                                                                                                                    
23. delay(1000);    
24. digitalWrite(motor1PinA, LOW);              //BACK                                                                                
25. digitalWrite(motor1PinB, HIGH);  
26. digitalWrite(motor2PinA, LOW);                                                                                                     
27. digitalWrite(motor2PinB, HIGH);                                                                                                                                    
28. delay(1000);    
29. digitalWrite(motor1PinA, HIGH);              //RIGHT                                                                                      
30. digitalWrite(motor1PinB, LOW);  
31. digitalWrite(motor2PinA, LOW);                                                                                                     
32. digitalWrite(motor2PinB, LOW);                                                                                                                                     
33. delay(1000);    
34. digitalWrite(motor1PinA, LOW);              //LEFT                                                                                       
35. digitalWrite(motor1PinB, LOW);  
36. digitalWrite(motor2PinA, HIGH);                                                                                                     
37. digitalWrite(motor2PinB, LOW);                                                                                                                                    
38.  delay(1000);    
}
