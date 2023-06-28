## What is this ?
This LeaderLine version is an extension to the original LeaderLine project https://github.com/anseki/leader-line .

## Why using it ?
The original leaderline class lacks:

* parent prop :

The original leaderline class always inserts the line svg element in body. Sometimes you want to insert the svg in a specific element.

* element prop : the svg element of the line

* absolute positioning : regradless of the parents scroll or offset.

## What's new ?
* New options :

* parent : where to insert the line element, default to document.body

* new Props :

* element : the line svg element

* Absolute positioning : even if the parent element changes position

* Scroll positioning : even if the start/end element exceeds the parent width/height and the parent becomes scrollable

## How to use it ?
Just install the current git repo using npm or any package manager of your choice :

> npm install --save github:AhmedAyachi/LeaderLine

And then use it in your code as follows : 
	
	import LeaderLine from "leaderline";
	
    const line=new LeaderLine({
	    //...OriginalClassProps,
	    parent:HTMLElement,
	    start:HTMLElement,
	    end:HTMLElement,
    });