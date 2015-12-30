Notes on starting mongo 
1)start terminal and type mongod 
2)start a new tab and type mongo  
 
 
 

 
You can't use build.sbt in Eclipse directly. Instead you need to generate an Eclipse project from your SBT project using sbteclipse plugin. Quoting the README:

Add sbteclipse to your plugin definition file. You can use either:

the global file (for version 0.13 and up) at ~/.sbt/0.13/plugins/plugins.sbt

the project-specific file at PROJECT_DIR/project/plugins.sbt

addSbtPlugin("com.typesafe.sbteclipse" % "sbteclipse-plugin" % "2.4.0")
In sbt use the command eclipse to create Eclipse project files

> eclipse
In Eclipse use the Import Wizard to import Existing Projects into Workspace

See the github wiki for more usage details. Don't forget to rerun eclipse command after changes in your SBT project.