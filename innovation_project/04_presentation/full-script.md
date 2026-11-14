# Innovation Project Script

JoyRobots Excavators · full script in speaking order.

Jayden → Lucas → Victor → Noah → Wilson → Kayden

---

## 1. Jayden · Identify

Did you know the Jefferson Salamander is endangered in Ontario? On cool, rainy spring nights, they walk from the forest to the pond, but Stouffville Road is in the way, and cars are a big danger to them. We visited Stouffville Road, where TRCA has studied salamanders since 2002. Tunnels were put under the road so salamanders can cross safely. Fences guide them to the tunnels, and cameras watch for animals going in. But something the experts still need to know is if salamanders are actually using the tunnels, because they could be turning back.

So we decided to help. Next, Lucas will explain our design.

---

## 2. Lucas · Design

What if we could use a sensor to count how many salamanders cross each year? We learned that TRCA's cameras can't always tell if a salamander turns back. We measured the real tunnel and made a sketch of it. The real tunnel is wet and has dirt in it, so our sensors have to stay dry. We decided to use an M5Stack and a ToF distance sensor looking down to track salamanders passing through. We put the sensor on top because if it is on the ground, the salamander would get scared and run away.

Next, Victor will talk about how we created it.

---

## 3. Victor · Create (tunnel model)

Imagine a salamander tunnel small enough to fit on a table. We built a tunnel replica. We took the sketch and turned it into a real model. We used a wooden base and top, a 3D printed tunnel, and clear acrylic sheets for the sides, so you can see inside. We decorated the top to look like the road. Together as a team, we screwed the bolts in to hold it together. Our tunnel is pretty accurate to the real one. The road and the tunnel match.

Now Noah will tell you about the M5Stack and sensors.

---

## 4. Noah · Create (M5Stack, sensors, code)

How does a tiny computer know a salamander is there? The ToF sensor is a laser that looks down and measures the distance to the floor, and it sends that number to the M5Stack. We programmed a rule using IF and THEN. IF something passes under the sensor and the distance gets shorter, THEN the screen says "Salamander found!" We 3D printed a model salamander to test it. As the salamander passes under the sensor, the distance number goes down and the screen shows "Salamander found!" It also counts every salamander that passes.

Next, Wilson will tell you how we tested it and made it better.

---

## 5. Wilson · Iterate

What happens when your invention does not work the first time? That happened to us. At first, we thought of using a motion sensor, but it looks for body heat and salamanders are cold-blooded, so it would not work. So we chose the ToF sensor, but our 3D printed salamander was a bit short and the sensor detected nothing. It also only detects a small spot, so we added more sensors. After many tests, we were able to consistently find the salamander. We also improved our design after an expert at TRCA, Dr. Ruppert, told us the tunnel must stay dark, cool and damp. Our sensors work in the dark, so they can add to what his cameras see.

Now off to Kayden to tell you how we shared our project.

---

## 6. Kayden · Communicate

We shared our project with two experts at TRCA, Dr. Jonathan Ruppert and Dr. David Lawrie. We sent them letters with our questions, then we showcased our project and got some feedback. Dr. Ruppert mentioned that if a salamander moves along the side of the tunnel, the sensors may not detect it. His feedback showed us we were right to add more sensors. Also, if there are other animals, the sensor may think they are salamanders. So we tuned our ToF sensor to look for a salamander's height.

By counting the salamanders that go through, we can help the experts prove if the tunnels really work, and help save salamanders' lives. So remember: the Jefferson Salamander is endangered in Ontario, and our sensors can help keep them safe. Thank you!
