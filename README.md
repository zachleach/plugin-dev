#	Plugin development initial setup
-	Rename the folders in the path to `Main.java` from `me/yourname/pluginname` to something like `me/zachleach/test`
-	Update the fields in the `src/resources/plugin.yml` file (`name` and `main`) to match your plugin name and path to main
-	Configure the `pom.xml` file for maven (see comments in the file)


#	Running the the server
-	Download Java 21 and add to PATH
-	Run the server jar file using the scripts I've provided (e.g., `./compile_jar` then `./start_script`, or `./recompile_repeat`)
-	If you're not on Linux, they probably won't work but the commands within those scripts will be approximately the same
-	Connect to the server with the ip `localhost:25565` (unless you modified the `server-ip` or `server-port` fields in the `server.properties` file)


#	Plugin/Server development
-	At a high level, plugin development is just writing Java statements you want to be executed whenever any in-game event occurs (e.g., when a player breaks a block, when a player issues a command, etc.)
-	My advice is to start by learning how to create a command and an Event Listener
-	The next thing would be learning how to schedule tasks (e.g., code that runs after X amount of seconds, or repeats Y amount of seconds); more concretely, go learn how to make custom particle animations
-	After that, it's a matter of just putting your mind to it and asking questions to ChatGPT (or back in my day, the Spigot/Bukkit plugin development forums)


#	Resources
-	Link to the functions you can use with the Spigot-API: https://hub.spigotmc.org/javadocs/bukkit/
-	Link to the functions you can use with the Paper-API: https://jd.papermc.io/paper/1.21.10/ (for example, Spigot-API doesn't have a PlayerJumpEvent but Paper-API does)
-	Link to the functions you can use for Chat related stuff with Paper-API: https://javadoc.io/doc/net.kyori/adventure-api/latest/index.html
-	I learned the plugin coding basics by watching `CodedRed` and `KodySimpson` on YouTube
-	I learned how to create/run a server so I can test my code by watching `TheBreakdownXYZ`


#	Tangentially-related technical advice
If you don't know these concepts, it's probably worth learning them at some point:
-	How do you compile and run a Java program using `java` and `javac` commands
-	What is a Jar file
-	What is maven and how do you use it to build and run a Java program
-	If you're on Windows and don't use WSL (Linux), force yourself to setup and use WSL and then run the server from there
