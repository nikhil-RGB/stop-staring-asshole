# stop_staring_asshole

![image](https://github.com/nikhil-RGB/stop-staring-asshole/assets/68727041/a9b94c01-c817-41bc-bb2c-2c957f3f9918)


> [!NOTE]  
> This <strong>"project"</strong> is all for shits and giggles. It's one goddamn screen lol.


## Purpose:

Ever had an asshole looking at your screen over your shoulder for longer than you're comfortable with? 
Here's a fun alternative: an "application" with just one screen, with a simple message: STOP STARING AT MY SCREEN, launched whenever you press a specefic key combination.
To use this "application":

- Clone the repo: ```git clone stop_staring_asshole```
- Navigate to the root directory of the project
- Once you are inside the stop_staring_asshole folder, you will have to build the application.
- build the application for your platform of choice(you will need to have flutter set up on your computer).

#### Run build command for windows:

```flutter build windows --release```

#### Run build command for linux:

```flutter build linux --release```

Alternatively, there is a [web deployment](https://stop-staring-asshole.web.app)

Once you've installed the app, you can use [auto-hotkey](https://www.autohotkey.com) (windows-only) to launch the app when a particular key or key combination is pressed.
An example of a AHK script which will launch the application if it is installed in "C:/personal" and ```CTRL+SHIFT+;``` is pressed.

```
#SingleInstance force
#NoEnv ; Performance reasons
; #Warn ; Warnings to ensure script correctness
SendMode Input ; Reliable
SetWorkingDir %A_ScriptDir% ; Ensure working directory consistency
^+;:: ; Extra trigger for stop staring asshole(CTRL+SHIFT+;)
Run, "C:\personal\stop_staring_asshole\build\windows\x64\runner\Release\stop_staring_asshole.exe"
return
```

If you'd like to launch the site in your browser instead, the script will look like this:

```
#SingleInstance force
#NoEnv ; Performance reasons
; #Warn ; Warnings to ensure script correctness
SendMode Input ; Reliable
SetWorkingDir %A_ScriptDir% ; Ensure working directory consistency
^+;:: ; Extra trigger for stop staring asshole(CTRL+SHIFT+;)
Run, "https://stop-staring-asshole.web.app"
return
```

In conclusion, I really hate it when people stare at my screen over my shoulder, and was bored out of my mind  so I threw together this shit. 🧑‍🎄
