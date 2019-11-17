# In-Game-Clock-Unity-Package
Highly customizable in game clock. You can customize almost everything without modifing the scripts.
There are two types of clock analog and digital.

<B>Setup</B>
<OL>
  <li>Import Package</li>
  <li>If asked for TextmeshPro, import it</li>
  <li>Goto Prefabs and just drop the clock prefab in to your scene</li>
</OL>
  That's it.

<B>Settings for clock</B>

![Setting](/Screenshot1.png)<BR><BR>
![Setting](/Screenshot2.png)

<OL>
  <li><B>Clock Type</B>
  <UL>
    <li>Has two options, for analog and digital clock.</li>
    <li><B>This option cannot be changed runtime.</B></li>
  </UL>
  <li><B>Use System Time</B>
    <UL>
    <li>If checked it will use the system time as the starting time, otherwise you can manually set starting time.</li>
    <li><B>This option cannot be changed runtime.</B></li>
  </UL>
  <li><B>Display Seconds</B>
    <UL>
    <li>If unchecked it won't show second hand in analog clock, and seconds in digital clock.</li>    
  </UL>
  <li><B>Time Speed</B>
  <UL>
    <li>Has two options, Hour for Day and Time scale.</li>
    <li>Hour for Day will allow you to specify how many real life hours will make one day in game.</li>
    <li>Time scale can be used as a multiplier, i.e. 1 will be real time, 2 means 2x faster and so on.</li>
  </UL>
  <li><B>Use 12 hour Format</B>
  
  <UL>
    <li>Only available if you select digital clock type.</li>
    <li>If checked it will display time in 12 hours format, otherwise 24 hours format.</li>    
  </UL>
</OL>

Furthermore, there are some Getter methods to get current in game time, all you have to do is grab reference of "ClockController" and you can use them as following

        private ClockController clockController;

        clockController.GetHours(); // returns int

        clockController.GetMinutes(); // returns int

        clockController.GetSeconds(); // returns int

        clockController.GetMeridiem(); // returns string
        
  Feel free to use it in your projects whether it is commercial or non-commercial. You don't even have to credit me either, however I'd love it if you do.
