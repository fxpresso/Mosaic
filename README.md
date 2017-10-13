# ![Mosaic Logo](http://metaware.us/images/mosaic.png)  
# Mosaic
The Ultimate JavaFX, Multi-split, Drag-n-Drop Layout Manager 

[![htm.java awesomeness](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](http://cogmission.ai)
***

## On [YouTube](https://youtu.be/eVH-Q85hqe0) (CLICK!)

Hi I'm an engineer for [Cortical.io](http://cortical.io), working on machine intelligence in the form of language intelligence - it's my dream situation and I have very little time other than that to forward the progress of this, but it is **too** substanstial to keep to myself! I'm hoping (with a lot of guidance from myself) that some enterprising Java engineer can take this and run with it! Please Please contact me if you're that person! cognitionmission@gmail.com...

# ![Demo](http://metaware.us/images/MosaicDemo.gif)

Mosaic is an **amazing** new layout manager which allows you to split your screen however you want with no nesting; Drag dividers in _**ANY**_ direction; and Drag-N-Drop contents anywhere, and the layout will intelligently morph into a new configuration while snapping to suggested locations!

OH YEAH...

Using Any Java Windowing Toolkit! (i.e. JavaFX, Swing, Apache Pivot etc.)

**Discerning Developer:** "Sounds cool... How does it do that!!!?"

Mosaic is an engine that furnishes dimensions and locations for objects it is given. So...

**Step 1:** Load it with objects in the same container (Could be string keys or some other mapping to your objects.) Mosaic doesn't operate on (i.e. resize or call any methods on) your objects. As a matter of fact it could be run on the server side!  
**Step 2:** Attach mouse listener to your container (albeit JavaFX Node, Swing or Apach Pivot Container); inside of which; forward events to the Mosaic Engine  
**Step 3:** Add a listener to Mosaic. Inside listener, apply location and dimension instructions to the object it tells you to... It will give you the object or mapping you furnished it with, plus a description of where to move or how to resize that object.

For examples for how this is done, see the MosaicPane reference classes in the "javafx", and "pivot" packages. (could be done the same way for Swing).

Easy peasy!

***

### To use Demos: (in the "src/test/java" source tree) 
**Runs on JavaFX _and_ Apache Pivot** (and anything else if you implement it yourself) 

1. Fork or clone repo
2. Setup in the IDE of your choice
3. Run the:
  * ai.cogmission.mosaic.refimpl.javafx.MosaicPaneRefImpl.java
  * ai.cogmission.mosaic.refimpl.javafx.SimpleTester.java
  * -- or --
  * ai.cogmission.mosaic.refimpl.pivot.MosaicPaneRefImpl.java
  * ai.cogmission.mosaic.refimpl.pivot.SimpleTester.java
4. All Dependencies are in "libs" directory.

***

### To Implement yourself: (in the "src/main/java" source tree)

Take a look at the  ai.cogmission.mosaic.refimpl.javafx.MosaicPane.java or  ai.cogmission.mosaic.refimpl.pivot.MosaicPane.java file for reference on how to implement your own container that can be managed by the Mosaic Engine.

**Better instructions are on the way... (we need your help!)**

***

### To Contribute: (This _**is**_ open source and free after all)

Contact me at: cognitionmission@gmail.com


