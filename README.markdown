# About Cocoa-Nu Template

The Cocoa-Nu Template combines Objective-C and Nu in one Cocoa application.  In essence, it combines all of the steps enumerated in [my blog post](http://www.fromconcentratesoftware.com/2008/05/24/mixing-nu-and-objective-c/) on mixing Nu and Objective-C.  With this template, you merely need to create a new Cocoa-Nu application and start coding.

# Why Objective-C + Nu?

Even though Nu is built on Objective-C and the Cocoa framework, there are some things that are just easier to do in Objective-C.  For instance, if you'd like to use a C library, it's probably easier to write an Obj-C wrapper than to wrap the functions in Nu.  Objective-C also compiles down while Nu remains interpreted.  While there probably won't be many major speed increases by using Objective-C over Nu, it's still nice to be able to write things in ObjC when you need to focus on resource management.

With this framework, there's no reason to choose one language over the other.  They can both be mixed in as first class components in a Cocoa application.

# What about header files?

Objective-C needs to be informed of any classes defined in Nu.  Since Objective-C uses header files for this type of introspection, I've written a small tool called [nug](http://github.com/Grayson/nug/tree/master).  nug will create these header files.

# What do I need to start using Cocoa-Nu?

You'll need Xcode and the [Nu framework](http://programming.nu).  Once Nu is installed, this template should take care of everything else you need.

# What does this template do?

This template does the following:

	1. Creates a new Xcode project with the Nu framework linked.
	2. The Nu framework is copied to the application's Frameworks folder and re-linked for easy distribution.
	3. Any Nu files found in the nu/ folder are automatically loaded on app launch.
	4. All necessary linker flags that suppress warnings when integrating Nu and Obj-C are set.

More information can be found [on my website](http://www.fromconcentratesoftware.com/2008/05/24/mixing-nu-and-objective-c/).

# Installing Cocoa-Nu

Copy the Cocoa-Nu folder to ~/Library/Application Support/Developer/Shared/Xcode/Project Templates/Application.

	mkdir -p ~/Library/Application\ Support/Developer/Shared/Xcode/Project\ Templates/Application
	cp -R Cocoa-Nu ~/Library/Application\ Support/Developer/Shared/Xcode/Project\ Templates/Application

# Contact info

[Grayson Hansard](mailto:info@fromconcentratesoftware.com)  
[From Concentrate Software](http://www.fromconcentratesoftware.com/)