# IoT-Project-Submission

My idea is a fire warning system that alerts the user of a fire or potential fire over Wifi on another device.


My timeline was such that I would spend week by week working on each componenent of the project. My timeline is this:

Week 1: Learning about what IoT is. 

I started researching about Iot before the meeting using different sources from the internet. Once I joined the class, I learned much more about Iot than any video i saw on youtube. With the basic knowledge gained from the meeting and a goal in mind, i decided to start thinking of what my project was going to be about. I was looking up the hardware specifications and tried to determine if my project ideas were feasable. I finsihe doff the week by narrowing downmy ideas and ordering the parts i wnated for my project.

Week 2: Downloading drivers and software for my projects. 

I began the week reading the very vague hookup guide. I downloaded all the drivers it asked me to and the libraries. I didnt do much this week becuase I was eagerly waiting for my haardware to arrive. I attacked all the packages that arrived and ripped them open to find that they arent what I was looking for.

Week 3: Setting up the hardware.

The day before the session, a red package arrived. In my typical fashion of grabbing and proceeding to rapidly rip open the packaging revealed to me what I was fawning over for the past week, the hardware!. I decided to set them up and research the code behind the hardware. Turns out, non of the drivers or libraries worked! I had to scour the internet and DISCORD for 3 hours! To find what I needed! I finally found out in a forum hidden deep within arduino. I downloaded everything I needed and started off with the blink code! 

Week 4: Learning about circuitry and more problems.

After the meeting, I followed what was going on in the meeting and used Tinkercad. I made a few neat circuits and explored more into the eletrical needs of the hardware. I saw that the easiest way to connect was the Qwiic connect wire, soI decided to use jumper cables! Which turns out that was a terrible idea becuase I kept doing the wrong things and it ceased to work. I decided to go the easy way after the end of the week and decide don my project idea. It was to detect fire around the house!

Week 5: Trying to use the sensors. 

After deciding to use the Qwicc connect system and figuring out my project idea, I move my way into using the sensor. The sensor did not work at all. It did not display anything and kept giving me errors. So i decided to hop on over to DISCORD! It didnt yield results so I donwloaded every library that had the keywords BME680 or BME688 in them. I found one that worked with the tedious strategy I used, but it was the end of the week before I discovered how to use it. 

Week 6: Trying to use the OLED

The process for this went about as similar as the sensor library process. The library given by the hooup guide did not work. "Surprise surprise"! I used the same method and DISCORD to find a library that worked. It worked almost flawlessly and I loved the OLED and thoguht of many ways to use it. I decided that I wanted my project to be about alerting about fire on the OLED. I messed around with it and decided to try and combine the sensor and OLED. 

Week 7: Combining the OLED and sensor

This task was much harder than any one I have had so far. The OLED would not display the values fromt he sensor. After some intense researching and time on DISCORD, I finally was able to get a value to display on the OLED. Which was a huge success! I tried to display temperature values and humidty next. I ran into another problem, I cant convert numerical vales to strings. I talked to many people on DISCORD and nothing worked. And yet again, dee in another Arduino forum, there lay our answer. A simple double string conversion. 

Week 8: Reading gas values and displaying them.

By the start of the week, I was able to display temperature and humidity on the OLED! I focused my attention on the gass vales now becuase they were key in detecting smoke. Turns out, the gas readings dont work! They are a static negative number. I spend hours and hours trying to solve this with the internet and DISCORD. My salvation came from Rushil explaining the Adafruit one can be fixed by changing a 77 to a 76. Which was a pain to realize and a miracle to obtain. I started testing the Adafruit library, which in fact it did work now. The gas would change when put in coffee or more importantly, smoke! 

Week 9: Guru Medetation Galore

The best week truned into the worst week in a single hour when I realized that the OLED does not work with the Adafruit library. When I searched this up, there were very vague answers and very disencouraging answers. I spent hours on DISCORD and forums trying to solve it. The OLED did not want to work with the Adafruit sensor. I spent a whole week trying to fix this or bypassing it. 

Week 10: Procrastination and a last minute project change

Turns out, the Adafruit library wont work with the OLED. My entire project was wrecked by a single error. I decided to only use humidity and temperature. I wasted a lot of time trying to fix the error instead of working on the actual code. On Thusday, I gaveup trying to fix it and foused on my code. Now it gives an alert when humidity is low and temperature is high. The last day was without incident in the morning. I was working on the finishing touches to my project when disaster struck. The power went out in my community. It cam back on instantly and I turned my PC back on to load Arduino, but as soon as I truned it on, it happned again. The power kept flickering on and off for an hour. I dont know what happened, but I lost some code. Once I retyped it, my nemesis apeared. The Guru Meditation error showed up. I could not use the OLED the only working library. I was on the verge of panic when I decided to calm down. I knew even if I kept trying, I could not fix the error. I was looking at the hookup guide when it mentioned usning Wif. And like a blaze I had an idea. What if I could sent a alert via Wifi to another persons device in case of a fire! I rapidly searched the Internet and I found a ton of resources on how to do it, but my time was running low. it was already 6:00. I rushed to write code to create a server that used my ESP32's IP to give a message. Using a bit of open-source code and made a ragtag way to do so. When a certain command is typed intot eh URL, it displays that message int eh serial monitor. Cool right! I used that code and put it into a condition that changed the resulting messgae that showed up on the user's screen to say of a fire if the sensor readings indicated so. I was so glad it worked when I ran it. I hastly rushed to make this report as I uploaded my code and sighed in relief. 

I aquired data inf roms of graphs and raw numbers. It does not allow me to post images of these so forgive me if I cannot include the actual data becuase it is too late to go looking for how. I interpreted the data using graphs and understanding why and how the trends occur in them. I noticed that the gas resistance tended to drop when exposed to different smells and in different amounts. Smoke decreased the gas value to less than ten while coffee only decreased it to 30. The raw data I interpreted using the serial moniter and researching the values. I learned what ohms were and I was able to analyze the data using this.

The results of this project was an alert being able to load into another persons device. 

My conclusion from this is that I learned many things and I am keen to learn more and test more. I also learned that there are many obstacles an errors that will come in your path. 

