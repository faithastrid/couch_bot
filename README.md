# couch_bot
couchbot from 2022 onwards

Couch Docs

We motorized a couch.

 

________________________________________

How to Use the Couch:

●	Sit on it, it's a couch
●	Turn on the couch by the main power switch in front (has labelled "on" and "off" positions; you can't go wrong).
●	Hit the emergency stop button (E-stop) (the red thing by the power switch) to immediately stop the motors. The other electronics (e.g., Raspberry Pi) will stay on; the E-stop only tells the motor drivers to not drive the motors anymore. Undo the E-stop by turning it until it pops out again, and the motor drivers will move the motors again.
●	How it's controlled depends on the programming at the moment, but right now (just after it's built, May 2019) there's a USB logitech dual action gamepad that plugs into the Raspberry Pi on the left side of the couch. When the couch power turns on, the Pi boots up and automatically runs a control program. The Y axes of the left and right gamepad joysticks are mapped to the speed of the left and right side wheels, respectively. If the gamepad USB cable becomes disconnected, the couch might stay moving and you probably want to hit the E-stop, turn off the couch, plug the joystick back in, and turn everything on again.
●	Charge the couch by plugging in the charger cable (stored on the right side of the couch) to the wall. ALWAYS TURN THE COUCH SWITCH OFF BEFORE CHARGING (running the motor drivers, Raspberry Pi, etc. could confuse the charger). It's a smart charger and these are well-behaved lead-acid batteries, so it's best to always keep the couch plugged in when not in use (charger will protect against overcharging) and drive it a bit once per month or so.
●	Battery life is probably 1-2 hours or more per charge.
●	Caster wheels can be deployed to, e.g., move the couch sideways through doors and into elevators. To deploy the caster wheels, first pull the footrest all the way out. Take the metal pipe with the orange rubber handle that is stored in the back of the couch, put it on the 3/4" threaded rod sticking out of the back of the couch on the right side, and push down to deploy the right caster wheels. Do the same in the front left for the left caster wheels. Now, to keep the caster wheels off the ground, while holding the left caster wheels up with the pipe, push in the footrest a bit. Then hold the right caster wheels up again and push in the footrest more. Finally, you can hold the left caster wheels up a little bit more and push in the footrest as far as it will go (so a hex nut is holding the left caster wheels up). Put the metal pipe back in the rear of the couch. To retract the caster wheels, do the same in reverse.
●	Keep the couch on caster wheels, not its drive wheels, when not in use. This is because the drive wheels currently squish a lot (see mechanical improvement project) and might be harmed if they are under load for a long time, but the caster wheels are designed for huge amounts of weight (900lb each, so ~ 4.5x safety factor).
●	The top of the couch (i.e., the actual couch plus a little bit of strut channel frame) lifts off to access the electronics. Lift this off by the strut channel sticking out of the left and right sides. This top bit attaches onto the bottom by resting on four pins in the four corners of the couch; it's held on by gravity.
●	There's a footrest. It holds retracted caster wheels (and also people's feet) off the ground.
●	All documents (this, BOM, CAD) are stored in the Demobots Google Drive, save software, which is on GitHub.

________________________________________

FAQ:

●	Why did we do this?
○	Because we can.
○	Why not?
○	We need classy transportation.
○	Biggest RAS robot yet! We beat IGVC for size.
○	Our demobots team was bored.
○	This is great for outreach; first time we drove it around, literally after 10pm the night we finished it, we got at least 3 people to seriously consider joining RAS (also see notes on EER opening demo in political background below). Also, this is perfect for UT orientation, Explore UT, and Introduce a Girl to Engineering Day. It just can't be brought off campus easily because ~500 lb. is really hard to move.
●	When did this project start?
○	Whoo, there's a long answer. The society dearly loves its furniture. In late November of 2012, RAS mounted a motorized wheel system to the communal couch. The couch was subsequently fitted with RGB LED lighting and a speaker system for the 2013 Red Bull Creation Contest. Relevant videos may be found here and there. And this was not even the first iteration: a similar couch, since lost to the ravages of time, was built in early 2010, as documented by this!
○	2017 (see blog http://ras.ece.utexas.edu/2017/04/17/couch.html): "The couch had not survived the interim until now well. It has not, to my knowledge, moved once in the past half decade under its own power—until now. For the past few months, a dedicated team of RAS furniture ninjas has unceasingly (technical term for ‘about one hour per week’) restored the couch to functional condition. This included unjamming a gearbox, rewiring the system (sorry, RAS alumni, but that hack you put together was not pretty), and writing some test code (found at GitHub). As a result of our tireless efforts, the couch now moves. We offer proof at YouTube. However, progress still needs to be made. The drive system has seen its best days, the couch upholstery is well past its prime, and, most shockingly, the couch boasts neither speakers nor lights! Thus, we hope to, after moving to our new home in the new UT Austin EERC building next year, redesign and rebuild the couch, properly, this time, to again make its fabled trip down Speedway street."
○	2019: the Demobot committee took on the couch! We took the red couch in the new IEEE office in the new EER building (which opened fall 2018) and designed a frame to fit from scratch. Everything was done to last: we spent ~$3000 on motors, electronics, and a lot of steel so it'd last a long time (we'll see how that goes) (funding is ~$500 from SEC, ~$2500 from RAS yearly budget from various companies). The project was started in the beginning of the fall semester, but only software was done (hats off to the software and phone app guys!) until the last month of the spring semester, when we finished the CAD, got funding, and ordered parts in a few weeks, then assembled the thing in a week The couch moved on the last days of the spring 2019 semester.
●	What's the political background of the couch?
○	The Cockrell dean (Sharon Wood) once expressed disdain at the ratty green couch (2012-2017 version) which, although comfortable, was still very ratty and jank.
○	However, despite these features and only half-functional, this couch was shown off at the opening of the EER, at which a few organizations (RAS, SAE, LRA) demonstrated projects to VIP funders. The couch was the favorite robot by far. 
○	Demobots wanted to rebuild the couch, and decided it too important to ignore. We took the couch in the IEEE office in the EER, without permission, since we didn't know who to ask, but took great pains to motorize it without modification (the couch is even held in place by rubberized bolts to prevent scratches!), so nobody can complain.
○	We believe that the couch is easily justifiable politically:
■	It's the EER's own furniture, so Cockrell can't complain it doesn't look good.
■	The frame is overengineered, professional-grade steel, looks great, etc.
■	Electronics are overengineered with integrated safety (e.g., E-stop).
■	It's a very effective outreach tool for Cockrell and RAS both.
○	Somewhat unrelated, Scott Evans, the director of the makerspace, loves the idea, though he might prefer the couch reupholstered in tacky orange. Might be able to combine couch with makerspace T-shirt cannon.
●	The couch weighs 500 lb, of which ~70 lb is the couch itself.
●	The couch cost $3000 (couch is free from EER, $500 motors + wheels, $300 batteries, $400 motor drivers, $1500 metal framing, a bit more misc.) 
●	Batteries are 2x12V, 55Ah lead acid for 24V, 55Ah total; motors probably draw about 10A each while running. Battery life is probably 1-2 hours (we haven't driven it long enough to find out!).
●	Motor drivers are 2 x "Sabertooth 2x60"; they can provide up to 60A/motor continuous, 120A/motor peak. Also have regenerative braking.
●	Motors + wheels are from a power wheelchair. They're ordered off eBay, since we didn't know how to order direct from manufacturer, and we have no idea what their torque curves, etc. are. Motors are about 350W each.
●	Our couch runs Linux
○	Control via Raspberry Pi Zero W, which runs a Python script on boot.
○	Control is currently via a USB joystick or a Bluetooth phone app.
○	The Pi sends commands over serial to the motor controllers.
●	What are particularly nifty features?
○	Deployable caster wheels to move sideways, e.g., through doorframes and elevators
○	Footrest
○	Our couch runs Linux
○	Wireless (bluetooth) phone control (almost done?)
○	Huge lead acid batteries for low-cost, heavy (we don't care), very long battery life
○	Reliability! Medical grade motors, steel frame, overengineered electronics. This should last for a very long time.
○	Metal strut channel is easy to add stuff onto
○	Top comes off bottom for easy maintenance

 

________________________________________

Potential Improvements to Work On:

MECHANICS

●	BUMPERS: zip-tie a cut pool noodle or cylindrical housing insulation along the left and right strut channel parts sticking out of the couch so that they won't scratch things they bump into.You'll need approximately one pool noodle. Preferably black, but red/orange/yellow might work well. UPDATE: done with some pipe insulation from Home Depot, which is black. It’s not very strong, though; pool noodles tear less easily. The next upgrade might be zip-tying on pool noodles instead, then stretching a fabric cover around them, a la bumpers for FIRST FRC bots.
●	TIRES: the tires currently on the couch are made of rubber and filled with foam. They're not meant to withstand the ~200 lb of a (50 lb couch + 150 lb people * 2)/(4 wheels), so they squish when moving, giving them more contact area with the ground, making them squeak horribly even more (the squeak comes from a slight sideways movement when the couch turns; going straight it's fine). Fortunately, I'm reasonably certain the motors are strong enough (they didn't come with many specs, but bariatric power chairs use similar motors for (500+ lb)/(2 wheels), so all we need to do is find better tires. Note that the wheels have 2 parts: the inner metal hub and the outer rubber/foam tire. The tire can be replaced while keeping the hub, and the tire's a standard size, so replacing it with something more heavy duty is easy. I *think* what we want is a solid urethane tire (like, solid plastic instead of foam-filled or air-filled (pneumatic)); these are used on, e.g., forklifts that have to carry lots of weight. So all we need to do is find some solid urethane tires the same size (so they fit) as the current ones, put them on the current wheel hubs, and we're done! (of course, this wouldn’t eliminate the sliding issue, just make the tires sufficiently strong withstand it.You can try building ginormous asphalt-ready omniwheels to replace the front wheels instead or something)
●	BRANDING: we need the couch to have "UT IEEE RAS" or "Robotics & Automation Society" or something on it so people know which club to join. :) Maybe use the makerspace vinyl cutter for white lettering along the side of the couch? Maybe the LED signboard?
●	SHELF: We can assemble (and have parts to do so) a shelf / table coming up from the left or right side of the couch to attach, e.g., a gaming joystick or user display or something.
●	LED LIGHT MOUNTING: we should put strips of LEDs (maybe addressable LEDs, e.g., neopixels) on the bottom of the couch. Be careful so that depolying/retracting the caster wheels won't squish them. (see electrical project for wiring, programming project for programming) UPDATE: NeoPixels are attached to the couch. Check the zip-ties and wiring to make sure it’s fastened onto the couch well and won’t get in the way of the moving parts (e.g., caster deployment).
●	SOUND: we should totally get some bluetooth speakers or something and wire it into the couch somehow. Some mechanical expertise is required to mount them so they're held on well and won't fall off easily. See electronics project.
●	LED SIGNBOARD: see detail in electronics section; this is a mechanical + electrical + software project.
●	REUPHOLSTERING: If the upholstering ever gets torn, Scott Evans, the director of the makerspace, may be willing to fund and has contacts for reupholstering the couch. He might be in favor of "tacky orange", although the red matches the caster wheels, switch, and e-stop.
●	BENT CASTER WHEEL HOLDER: The bar on the footrest that holds the right caster wheel in place was bent. The caster wheel system collapsed and bent the bar when it got stuck exiting the elevator. We need to unbend the bar and think about how to secure the caster wheels when they hit bumps.

ELECTRONICS

●	POWER ELECTRONICS: the couch runs off of 24V provided by two 12V batteries in series. However, we will probably need 12V for, e.g., LED strips. We should always keep the batteries in series so they charge and discharge at the same rate (i.e., let's not get 12V by connecting to only one battery), so we need to put on a 12V voltage regulator. How about this:
○	get 5V and 12V voltage regulators with sufficient current output for whatever LEDs, etc. we want to have (e.g., maybe this for ~15A loads)
○	24V input to the regulators should be connected the same way as the motor drivers (i.e., to the battery ground terminal and the fuse positive terminal)
○	output from the voltage regulators  
○	just for fun, we could get an AC inverter, power it off 24V, and be able to plug in things like laptops
○	Update: there is currently a 5v5A Pololu voltage regulator powering the NeoPixels. This eventually gets hot, and we might want a 5V regulator with higher current max
●	CONTROL ELECTRONICS CIRCUIT BOARD / ENCLOSURE: The Raspberry Pi is literally just taped onto the couch right now with some soldered connections. We could make a nice circuit board and enclosure to pretty things up a bit. This is a good time to add in the power electronics voltage regulators, LED connections, etc. 
●	LED SIGNBOARD: we could take the LED signboard, build it a new frame out of strut channel (i.e. https://www.mcmaster.com/struts, the same stuff we built the couch frame out of) (frankly, the current wooden backing is a little cheap), and make it so that we can attach it to the back of the couch (but also removable, so we can bring it places without bringing the whole couch) (okay, this part's also a lot of mechanical work; see mechanical project). Power can be 12V from the couch or maybe mains AC so we can plug it into the wall or into an AC inverter on the couch. (programming the signboard is also a lot of programming work; see programming project)
●	LED LIGHT WIRING: we should put strips of LEDs (maybe addressable LEDs, e.g., neopixels) on the bottom of the couch (see mechanical project). These will probably have to be wired into a 12V voltage regulator (see power electronics project). We could use solid color LED strips, but those are boring. Addressable LEDs are really cool, but need to be wired up to a Raspberry Pi or something and then programmed (see programming project). UPDATE: NeoPixels are zip-tied to the couch. At full power, they may be drawing too much current from the 12V regulator they’re attached to, making it heat up---confirm this, and, if need be, replace the regulator. Also, put ring terminals on the power input to the voltage regulator to attach it to the power system like the motor drivers (i.e., battery ground terminal and the positive terminal on the fuse) instead of sticking wires into a motor driver battery input.
●	SOUND: we should totally get some bluetooth speakers or something and wire it into the couch somehow (see mechanical project). Bluetooth is nice because most of our music is stored on our smartphones nowadays, and some of those don't have audio jacks, and bluetooth speakers are common. Hooking these up to the Raspberry Pi controlling the couch is probably more trouble than it's worth (hence this isn't a programming project) because we'd switch between sounds from the Pi and music from a phone, but IDK, maybe we want to do even that?
●	GAMING JOYSTICK: wire up the Logitech 3D Pro gaming joystick to a shelf (see mechanical project) on the couch! This should be easy; just a USB cable to the Pi. The rest is programming (see programming project). 
●	E-STOP INDICATOR LIGHT: light that turns on when the E-Stop is pressed, sometimes it is hard to tell when it is engaged
●	LCD SCREEN OR RASPBERRY PI DESKTOP DISPLAY: Add a screen so the Pi can display some information to the rider, or give them access to the Raspberry Pi GUI. This could be attached near the joystick
○	Possible simple LCD screen - https://pimylifeup.com/raspberry-pi-lcd-16x2/
●	ADDITIONAL CONTROLLERS: Hardware receivers for additional controllers, such as radio. 
●	** COLLISION DETECTION SYSTEM: Use distance or object sensors to create detect when the couch is about to collide with a person or object, and halt the couch. This would make the couch a lot safer. Hardware and software. 
●	SPEED GAUGE: Add hardware, such as motor encoders or an IMU, that can determine speed or be used for PID control of the Left/Right speed

PROGRAMMING (see https://github.com/ut-ras/couch-pi )

●	BLUETOOTH CONTROL: People often ask if we can control the couch with our phones. Raspberry Pi bluetooth + phone app! (though we still also want a wired controller for reliability). This is in progress. 
○	The app and bluetooth communication work, now we need to set up the wired controller to operate at the same time and take over in case of emergency. 
○	add NeoPixel controls to the app
○	Test the app on multiple devices.
●	GAMING JOYSTICK CONTROL: We have a Logitech Extreme 3D Pro gaming joystick. If we wire it up to the couch on a shelf (see mechanical project), then all anyone has to do to use the couch is turn it on and use the joystick, no USB gamepad with long cables or bluetooth phone apps that may not be set up right to worry about! This is a convenience feature (the simpler the couch is to use, the easier it is for any of us to run at demos), a safety feature (USB cable gamepads and phone apps can disconnect while the couch is running, but if this joystick physically mounted on the couch always overrides any other controls, the person riding it will have some control over the couch besides just the emergency stop button), and coolness factor (joystick with trigger. Extra buttons to sync with LEDs and sound. 'nuff said). 
●	LED LIGHT CONTROL: We put addressable RGB LEDs on the couch; program these! Light up LEDs when the couch moves, is turning, reverses, joystick buttons, etc. (see mechanical, electrical projects). These will probably be controlled via Raspberry Pi GPIO.    pi/Drivers/Led.py
○	Currently there are 3 status LEDs and a NeoPixel strip. There are two NeoPixel functions, we need more
○	Turn signals using the LED strip
●	LED SIGNBOARD CONTROL: see detail in electronics section; this is a mechanical + electrical + software project.
●	SMOOTHER STOPPING: Determine the deceleration value based on the current speed at the moment when the stop button is hit. Currently, there is a fixed deceleration for the hard stop. pi/Drivetrains/TankDrivetrainAcceleration.py
●	SOFTWARE PORTS: Advanced software project. Migrate the couch control library to another system. This can be a different framework on the Raspberry Pi or another non-Linux based microcontroller. Examples include implementing on an RTOS, using ROS, or another microcontroller such as TM4C or ESP32.
●	** COLLISION DETECTION SYSTEM: Use distance or object sensors to create detect when the couch is about to collide with a person or object, and halt the couch. This would make the couch a lot safer. Hardware and software. 
●	TIMING PROFILE OF THE COUCH: use GPIO pins and a logic analyzer to profile the performance of the couch - controller response time, thread behavior, etc. We want to minimize controller latency, so the couch wheels move as soon as, e.g., a joystick is pressed. Previously, there was some kind of issue with the motor driver commands getting stuck in serial flush for 0.1 seconds, which, when fixed, according to Cole, changed to about 0.005s and is a very noticeable difference. Note we use the Python threading library, which doesn’t actually run multiple threads, but this is ok because the program is I/O bound, not CPU bound.

UPDATES (May 15, 2022)
●	Couch was fixed and back in working condition
●	Code was rewritten and motors were taken apart 
●	Bearing for the front left (if you were sitting on the couch) motor needs to replaced (21009 bearing)

UNCATEGORIZED:

●	Speed gauge
●	Battery power gauge
●	GPS
●	Cupholders / tray
●	Control panel for controller, speed gauge, light/speaker controls, and emergency shutoff
●	License plate
●	Distance sensors and automation
●	Time Travel
○	Flux capacitor


