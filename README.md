Slides for Intro to Scala Talk from Brighton Java
=================================================

These slides accompanied the talk *An Introduction to Scala* by Dave Gurnell and Richard Dallaway,
given at [BrightonJava](http://www.brightonjava.com) on 7th August 2013. The talk abstract follows:

> Dave Gurnell and Richard Dallaway present a brief introduction to [Scala](http://scala-lang.org) –
> a powerful programming language for the JVM. In the talk, the speakers introduce
> Scala from a Java programmer’s perspective, and show how its support for object-oriented
> and functional programming styles can provide a smooth transition to greater productivity
> and code reliability.

The slides are implemented as interactive *Scala Worksheets* in the Scala IDE for Eclipse.
Full instructions on getting started are provided below.

For a more representative example of a real application written using Java and Scala, see the
companion Git repository: https://github.com/davegurnell/brighton-java-sample-app

Viewing the Code
================

The source code for the slides is in the `src/main/scala` folder. The files are *Scala Worksheets*
sources (as opposed to regular Scala sources). Scala Worksheets is a plugin for Eclipse that shows
Scala code side-by-side with the output from compiling and running the code. We recommend you view
the files using the Eclipse tools so you can try things out and bounce ideas off the compiler.

Installing Scala IDE for Eclipse
================================

The project is built using [SBT](http://scala-sbt.org). To view the code in the Eclipse IDE:

 0. Install the Scala plugin for Eclipse. The simplest way to do this is to download the 
    pre-packaged *Scala IDE* bundle from [http://scala-ide.org], which includes both Eclipse itself
    and the Scala plugin in a single archive.

 1. Clone the git repo and change to its root directory:

        git clone https://github.com/davegurnell/brighton-java-scala-talk.git
        cd brighton-java-scala-talk

 2. Run the `sbt eclipse` script to generate Eclipse configuration files. The first time you run 
    SBT it may take some time to download and cache JAR files on your hard drive 
    (look in `~/.ivy2` if you want to delete them later):

        ./sbt.sh eclipse

 3. Import the code as an Eclipse project by selecting **File menu / Import... / General / Existing
    Projects into Workspace** and selecting the root directory of the repo.
