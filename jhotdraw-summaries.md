<h2>JHotDraw</h2>
<p>A Java-based drawing framework and application that provides a collection of packages for creating, manipulating, and managing drawings in a graphical user interface, along with utility classes and interfaces for various functionalities.</p>
<h3>Packages:</h3>
<ul>
<li><p><strong>CH.ifa.draw.applet</strong>: Initialize and manage the DrawApplet class and load icons and display status messages at regular intervals.</p></li>
<details><summary>Subgoals:</summary>
<ul>
<li><p><strong>Manage DrawApplet</strong>: Initialize and manage the DrawApplet class.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.applet.DrawApplet</strong>: Initialize and manage the DrawApplet class.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>View management</strong>: Return the drawing view of the DrawApplet class.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>view()</strong>: Return the drawing view of the DrawApplet class.</p></li>
</ul>
</details>
<li><p><strong>Initialization</strong>: Initialize the DrawApplet by creating and setting up the necessary components and panels.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>init()</strong>: Initialize the DrawApplet by creating and setting up the necessary components and panels.</p></li>
</ul>
</details>
<li><p><strong>Selection management</strong>: Set up the attributes for the drawing view when the selection is changed.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>selectionChanged(CH.ifa.draw.framework.DrawingView)</strong>: Set up the attributes for the drawing view when the selection is changed.</p></li>
</ul>
</details>
<li><p><strong>Drawing management</strong>: Return the current drawing object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawing()</strong>: Return the current drawing object.</p></li>
</ul>
</details>
<li><p><strong>Tool management</strong>: Return the current tool being used in the DrawApplet class.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>tool()</strong>: Return the current tool being used in the DrawApplet class.</p></li>
</ul>
</details>
<li><p><strong>Palette management</strong>: Set the selected tool and name based on the user-selected palette button.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>paletteUserSelected(CH.ifa.draw.util.PaletteButton)</strong>: Set the selected tool and name based on the user-selected palette button.</p></li>
</ul>
</details>
<li><p><strong>Status message management</strong>: Set the status message to the name of the button if the user is hovering over it, otherwise set it to the name of the selected tool button.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>paletteUserOver(CH.ifa.draw.util.PaletteButton,boolean)</strong>: Set the status message to the name of the button if the user is hovering over it, otherwise set it to the name of the selected tool button.</p></li>
</ul>
</details>
<li><p><strong>Tool completion</strong>: Set the default tool and select it.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>toolDone()</strong>: Set the default tool and select it.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Manage SleeperThread</strong>: Load icons and display status messages at regular intervals.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.applet.SleeperThread</strong>: Load icons and display status messages at regular intervals.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Display status messages</strong>: Display a status message every 50 milliseconds until interrupted.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>run()</strong>: Load icons and display a status message every 50 milliseconds until interrupted.</p></li>
</ul>
</details>
<li><p><strong>Load icons</strong>: Load icons.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>run()</strong>: Load icons and display a status message every 50 milliseconds until interrupted.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>CH.ifa.draw.application</strong>: Create and manipulate drawings using the DrawApplication class in the CH.ifa.draw.application package.</p></li>
<details><summary>Subgoals:</summary>
<ul>
<li><p><strong>Create and manipulate drawings</strong>: Allows users to create and manipulate drawings</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.application.DrawApplication</strong>: Represents a DrawApplication that allows users to create and manipulate drawings.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>User Interface</strong>: Handle user interactions with the application's user interface.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>view()</strong>: Return the drawing view of the DrawApplication.</p></li>
<li><p><strong>print()</strong>: Prints the drawing to a printer.</p></li>
<li><p><strong>open()</strong>: Open the DrawApplication by initializing the necessary components and displaying the application window.</p></li>
<li><p><strong>exit()</strong>: Exit the application by destroying it, making it invisible, disposing it, and then exiting the system.</p></li>
</ul>
</details>
<li><p><strong>File Operations</strong>: Handle file operations such as saving, opening, and creating new drawings.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>promptSaveAsSerialized()</strong>: Prompt the user to save the file as a serialized object and save it if a valid path is provided.</p></li>
<li><p><strong>toolDone()</strong>: Set the default tool and select it.</p></li>
<li><p><strong>drawing()</strong>: Return the drawing object associated with this DrawApplication.</p></li>
<li><p><strong>promptSaveAs()</strong>: Prompt the user to save the file with a specified path and format.</p></li>
<li><p><strong>tool()</strong>: Return the current tool being used in the DrawApplication.</p></li>
<li><p><strong>promptOpen()</strong>: Open a file dialog to prompt the user to select a file, and load the selected file into the drawing.</p></li>
<li><p><strong>promptNew()</strong>: Initialize a new drawing.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>User Interface</strong>: Provides the user interface for the DrawApplication</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.application.DrawApplication</strong>: Represents a DrawApplication that allows users to create and manipulate drawings.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>User Interface</strong>: Handle user interactions with the application's user interface.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>view()</strong>: Return the drawing view of the DrawApplication.</p></li>
<li><p><strong>print()</strong>: Prints the drawing to a printer.</p></li>
<li><p><strong>open()</strong>: Open the DrawApplication by initializing the necessary components and displaying the application window.</p></li>
<li><p><strong>exit()</strong>: Exit the application by destroying it, making it invisible, disposing it, and then exiting the system.</p></li>
</ul>
</details>
<li><p><strong>File Operations</strong>: Handle file operations such as saving, opening, and creating new drawings.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>promptSaveAsSerialized()</strong>: Prompt the user to save the file as a serialized object and save it if a valid path is provided.</p></li>
<li><p><strong>toolDone()</strong>: Set the default tool and select it.</p></li>
<li><p><strong>drawing()</strong>: Return the drawing object associated with this DrawApplication.</p></li>
<li><p><strong>promptSaveAs()</strong>: Prompt the user to save the file with a specified path and format.</p></li>
<li><p><strong>tool()</strong>: Return the current tool being used in the DrawApplication.</p></li>
<li><p><strong>promptOpen()</strong>: Open a file dialog to prompt the user to select a file, and load the selected file into the drawing.</p></li>
<li><p><strong>promptNew()</strong>: Initialize a new drawing.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>File Operations</strong>: Handles file operations for the DrawApplication</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.application.DrawApplication</strong>: Represents a DrawApplication that allows users to create and manipulate drawings.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>User Interface</strong>: Handle user interactions with the application's user interface.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>view()</strong>: Return the drawing view of the DrawApplication.</p></li>
<li><p><strong>print()</strong>: Prints the drawing to a printer.</p></li>
<li><p><strong>open()</strong>: Open the DrawApplication by initializing the necessary components and displaying the application window.</p></li>
<li><p><strong>exit()</strong>: Exit the application by destroying it, making it invisible, disposing it, and then exiting the system.</p></li>
</ul>
</details>
<li><p><strong>File Operations</strong>: Handle file operations such as saving, opening, and creating new drawings.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>promptSaveAsSerialized()</strong>: Prompt the user to save the file as a serialized object and save it if a valid path is provided.</p></li>
<li><p><strong>toolDone()</strong>: Set the default tool and select it.</p></li>
<li><p><strong>drawing()</strong>: Return the drawing object associated with this DrawApplication.</p></li>
<li><p><strong>promptSaveAs()</strong>: Prompt the user to save the file with a specified path and format.</p></li>
<li><p><strong>tool()</strong>: Return the current tool being used in the DrawApplication.</p></li>
<li><p><strong>promptOpen()</strong>: Open a file dialog to prompt the user to select a file, and load the selected file into the drawing.</p></li>
<li><p><strong>promptNew()</strong>: Initialize a new drawing.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>CH.ifa.draw.contrib</strong>: Provides classes for drawing and manipulating polygon, diamond, and triangle figures.</p></li>
<details><summary>Subgoals:</summary>
<ul>
<li><p><strong>Manipulating and interacting with polygon figures</strong>: This subgoal involves classes that provide methods for manipulating and interacting with polygon figures.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.contrib.PolygonFigure</strong>: Represents a polygon figure and provides methods for manipulating and interacting with it.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Point Manipulation</strong>: Methods for adding, inserting, setting, removing, and retrieving points in the polygon figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>addPoint(int,int)</strong>: Add a point to the polygon figure at the specified coordinates.</p></li>
<li><p><strong>insertPointAt(java.awt.Point,int)</strong>: Inserts a new point at the specified index in the polygon figure, updating the polygon's points accordingly.</p></li>
<li><p><strong>setPointAt(java.awt.Point,int)</strong>: Set the coordinates of the specified point in the polygon figure to the given x and y values.</p></li>
<li><p><strong>removePointAt(int)</strong>: Remove the point at the specified index from the polygon figure.</p></li>
<li><p><strong>pointAt(int)</strong>: Return the point at the specified index in the polygon.</p></li>
<li><p><strong>points()</strong>: Return an enumeration of the points that make up the polygon figure.</p></li>
<li><p><strong>pointCount()</strong>: Return the number of points in the polygon figure.</p></li>
</ul>
</details>
<li><p><strong>Segment Manipulation</strong>: Methods for finding, splitting, and smoothing segments of the polygon figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>findSegment(int,int)</strong>: Find the segment of the polygon figure that is closest to the given coordinates.</p></li>
<li><p><strong>splitSegment(int,int)</strong>: Split the segment of the polygon figure at the specified coordinates and return the index of the newly inserted point.</p></li>
<li><p><strong>smoothPoints()</strong>: Smooths the points of the polygon figure by removing points that are too close to the line formed by their neighboring points.</p></li>
</ul>
</details>
<li><p><strong>Geometry Calculation</strong>: Methods for calculating the center point, bounding box, and distance from a line of the polygon figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>center()</strong>: Calculate and return the center point of the polygon figure.</p></li>
<li><p><strong>getPolygon()</strong>: Return a new `java.awt.Polygon` object with the x and y coordinates of the polygon and the number of points.</p></li>
<li><p><strong>bounds(java.awt.Polygon)</strong>: Calculate the bounding rectangle of a given polygon.</p></li>
<li><p><strong>center(java.awt.Polygon)</strong>: Calculate and return the center point of the given polygon.</p></li>
<li><p><strong>distanceFromLine(int,int,int,int,int,int)</strong>: Calculate the distance between a point and a line segment.</p></li>
</ul>
</details>
<li><p><strong>Drawing and Display</strong>: Methods for drawing, filling, and displaying the polygon figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawFrame(java.awt.Graphics)</strong>: Draws the outline of the polygon figure using the specified graphics context.</p></li>
<li><p><strong>drawBackground(java.awt.Graphics)</strong>: Fill the polygon with the specified background color.</p></li>
<li><p><strong>displayBox()</strong>: Return the bounding rectangle that encloses the polygon figure.</p></li>
</ul>
</details>
<li><p><strong>Interaction and Manipulation</strong>: Methods for checking containment, creating handles and connectors, and scaling/rotating the polygon figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>containsPoint(int,int)</strong>: Check if the given point (x, y) is contained within the polygon figure.</p></li>
<li><p><strong>handles()</strong>: Create and return a vector of handles for the polygon figure.</p></li>
<li><p><strong>connectorAt(int,int)</strong>: Return a connector at the specified coordinates in the polygon figure.</p></li>
<li><p><strong>scaleRotate(java.awt.Point,java.awt.Polygon,java.awt.Point)</strong>: Scale and rotate a polygon figure around a given anchor point.</p></li>
<li><p><strong>chop(java.awt.Polygon,java.awt.Point)</strong>: Chops the given polygon at the closest point to the given point and returns the coordinates of the chop point.</p></li>
<li><p><strong>chop(java.awt.Point)</strong>: Chops the given point on the polygon figure and returns the resulting point.</p></li>
<li><p><strong>isEmpty()</strong>: Check if the polygon figure is empty by determining if the number of points is less than 3 or if the width and height are both less than a certain threshold.</p></li>
<li><p><strong>outermostPoint()</strong>: Return the outermost point of the polygon figure.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Methods for reading and writing the polygon figure to a storable output.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the polygon figure and its points to the specified storable output.</p></li>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the data from the input stream and reconstructs the polygon figure.</p></li>
</ul>
</details>
<li><p><strong>Utility</strong>: Methods for basic movement and resizing of the polygon figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>basicMoveBy(int,int)</strong>: Move the polygon figure by the specified amount in the x and y directions.</p></li>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Move and resize the polygon figure to fit within the specified origin and corner points.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.contrib.PolygonScaleHandle</strong>: This class represents a handle for scaling and rotating a polygon figure.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Scaling and rotating</strong>: Scale and rotate the polygon figure based on the given step values and the current drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invokeStep(int,int,CH.ifa.draw.framework.Drawing)</strong>: Scale and rotate the polygon figure based on the given step values and the current drawing.</p></li>
</ul>
</details>
<li><p><strong>Resetting</strong>: Reset the original polygon, origin, and current position to null.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invokeEnd(int,int,CH.ifa.draw.framework.Drawing)</strong>: Reset the original polygon, origin, and current position to null.</p></li>
</ul>
</details>
<li><p><strong>Initialization</strong>: Initialize the necessary variables for scaling a polygon handle.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invokeStart(int,int,CH.ifa.draw.framework.Drawing)</strong>: Initialize the necessary variables for scaling a polygon handle.</p></li>
</ul>
</details>
<li><p><strong>Locating</strong>: Return the current point if it exists, otherwise return the origin point.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>locate()</strong>: Return the current point if it exists, otherwise return the origin point.</p></li>
</ul>
</details>
<li><p><strong>Drawing</strong>: Draws a yellow filled oval and a black outlined oval using the given graphics object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws a yellow filled oval and a black outlined oval using the given graphics object.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.contrib.PolygonHandle</strong>: Represents a handle for manipulating a polygon shape.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Locating the handle</strong>: Returns the location of the polygon handle.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>locate()</strong>: Return the location of the polygon handle.</p></li>
</ul>
</details>
<li><p><strong>Setting the handle point</strong>: Sets the point at the specified coordinates in the polygon handle.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invokeStep(int,int,int,int,CH.ifa.draw.framework.DrawingView)</strong>: Set the point at the specified coordinates in the polygon handle.</p></li>
</ul>
</details>
<li><p><strong>Smoothing the handle points</strong>: Smooths the points of the polygon handle when the user finishes invoking the method.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invokeEnd(int,int,int,int,CH.ifa.draw.framework.DrawingView)</strong>: Smooths the points of the polygon handle when the user finishes invoking the method.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Drawing and managing diamond figures</strong>: This subgoal involves classes that draw and manage diamond figures.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.contrib.DiamondFigure</strong>: Draws and manages a diamond figure.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Drawing</strong>: Draws a diamond figure with the specified fill color and frame color.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws a diamond figure with the specified fill color and frame color.</p></li>
</ul>
</details>
<li><p><strong>Containment</strong>: Checks if the given point (x, y) is contained within the diamond figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>containsPoint(int,int)</strong>: Check if the given point (x, y) is contained within the diamond figure.</p></li>
</ul>
</details>
<li><p><strong>Connection Insets</strong>: Calculates and returns the connection insets for the DiamondFigure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectionInsets()</strong>: Calculate and return the connection insets for the DiamondFigure.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Drawing polygons and managing polygon tools</strong>: This subgoal involves classes that handle drawing polygons and managing polygon tools.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.contrib.PolygonTool</strong>: This class represents a tool for drawing polygons.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Handling mouse events</strong>: Handles mouse events such as mouse down, mouse up, mouse move, and mouse drag to interact with the polygon being drawn.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseDown(java.awt.event.MouseEvent,int,int)</strong>: Smooths the points of the polygon and ends the tool if the mouse is double-clicked, otherwise adds a new point to the polygon.</p></li>
<li><p><strong>mouseUp(java.awt.event.MouseEvent,int,int)</strong>: Handle the event when the mouse button is released at the specified coordinates.</p></li>
<li><p><strong>mouseMove(java.awt.event.MouseEvent,int,int)</strong>: Update the position of the last point in the polygon to the given coordinates and refresh the view.</p></li>
<li><p><strong>mouseDrag(java.awt.event.MouseEvent,int,int)</strong>: Add the coordinates of the mouse drag event to the polygon being drawn.</p></li>
</ul>
</details>
<li><p><strong>Activating and deactivating the tool</strong>: Activates and deactivates the polygon tool by resetting the fPolygon variable and removing the polygon from the drawing if necessary.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>activate()</strong>: Activate the PolygonTool by resetting the fPolygon variable to null.</p></li>
<li><p><strong>deactivate()</strong>: Deactivates the polygon tool and removes the polygon from the drawing if it has less than 3 points or a width or height less than 4.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Drawing and manipulating triangle figures</strong>: This subgoal involves classes that draw and manipulate triangle figures.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.contrib.TriangleRotationHandle</strong>: Draws and manipulates a triangle rotation handle.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Drawing</strong>: Draws the rotation handle on the canvas.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws a yellow filled oval and a black outlined oval using the given graphics object.</p></li>
</ul>
</details>
<li><p><strong>Locating</strong>: Returns the origin point of the rotation handle.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>locate()</strong>: Return the origin point of the triangle rotation handle.</p></li>
</ul>
</details>
<li><p><strong>Rotating</strong>: Rotates the triangle figure by a specified angle.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invokeStep(int,int,CH.ifa.draw.framework.Drawing)</strong>: Rotate the triangle figure by the specified angle.</p></li>
</ul>
</details>
<li><p><strong>Resetting</strong>: Resets the origin and center points of the rotation handle.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invokeEnd(int,int,CH.ifa.draw.framework.Drawing)</strong>: Reset the origin and center points of the triangle rotation handle.</p></li>
</ul>
</details>
<li><p><strong>Initializing</strong>: Initializes the center and origin variables of the rotation handle.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invokeStart(int,int,CH.ifa.draw.framework.Drawing)</strong>: Initialize the center and origin variables of the TriangleRotationHandle object with the given x and y coordinates and the drawing object.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.contrib.TriangleFigure</strong>: Represents a triangle figure that can be rotated and manipulated.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Connection Insets</strong>: Calculate and return the connection insets for the triangle figure based on its rotation.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectionInsets()</strong>: Calculate and return the connection insets for the triangle figure based on its rotation.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Write and read the rotation value of the TriangleFigure object to/from a StorableOutput/StorableInput.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the rotation value of the TriangleFigure object to the specified StorableOutput.</p></li>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the rotation value from the given StorableInput and assigns it to the fRotation variable.</p></li>
</ul>
</details>
<li><p><strong>Containment</strong>: Check if a given point is contained within the triangle figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>containsPoint(int,int)</strong>: Check if the given point is contained within the triangle figure.</p></li>
</ul>
</details>
<li><p><strong>Cloning</strong>: Clone the TriangleFigure object and set the rotation value before returning the cloned object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>clone()</strong>: Clone the TriangleFigure object and set the rotation value before returning the cloned object.</p></li>
</ul>
</details>
<li><p><strong>Polygon Creation</strong>: Create and return a polygon based on the rotation of the triangle figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>polygon()</strong>: Create and return a polygon based on the rotation of the triangle figure.</p></li>
</ul>
</details>
<li><p><strong>Handle Addition</strong>: Add a triangle rotation handle to the vector of handles for the TriangleFigure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Add a triangle rotation handle to the vector of handles for the TriangleFigure.</p></li>
</ul>
</details>
<li><p><strong>Rotation</strong>: Rotate the triangle figure by the specified angle.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>rotate(double)</strong>: Rotate the triangle figure by the specified angle.</p></li>
</ul>
</details>
<li><p><strong>Drawing</strong>: Draw a filled and outlined polygon using the given graphics context.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws a filled and outlined polygon using the given graphics context.</p></li>
</ul>
</details>
<li><p><strong>Center Calculation</strong>: Calculate and return the center point of the triangle figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>center()</strong>: Calculate and return the center point of the triangle figure.</p></li>
</ul>
</details>
<li><p><strong>Chopping</strong>: Chop the given point on the triangle figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>chop(java.awt.Point)</strong>: Chops the given point on the triangle figure.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>CH.ifa.draw.figures</strong>: Provides a collection of classes for drawing and manipulating figures in a Java application.</p></li>
<details><summary>Subgoals:</summary>
<ul>
<li><p><strong>Figure Manipulation</strong>: Manipulating and retrieving attributes of figures</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.figures.FigureAttributes</strong>: Represents the attributes of a figure and provides methods to manipulate and retrieve these attributes.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Attribute Manipulation</strong>: Methods to set, get, and check the existence of attributes in the FigureAttributes map.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>set(java.lang.String,java.lang.Object)</strong>: Set the value of the specified attribute with the given name.</p></li>
<li><p><strong>get(java.lang.String)</strong>: Return the value associated with the specified name from the map.</p></li>
<li><p><strong>hasDefined(java.lang.String)</strong>: Check if the specified name is defined in the FigureAttributes map.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Methods to write and read the attributes of a figure to/from a StorableOutput/StorableInput object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the attributes of the figure to the given StorableOutput object.</p></li>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the attributes of a figure from a StorableInput object and stores them in a Hashtable.</p></li>
</ul>
</details>
<li><p><strong>Cloning</strong>: Method to create a clone of the FigureAttributes object and its associated Hashtable.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>clone()</strong>: Clone the FigureAttributes object and its associated Hashtable, and return the cloned object.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Handle Manipulation</strong>: Drawing and manipulating handles for figures</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.figures.RadiusHandle</strong>: Draws and manipulates a radius handle for a figure with an arc.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Drawing</strong>: Draws a yellow filled oval and a black outline oval using the given graphics object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws a yellow filled oval and a black outline oval using the given graphics object.</p></li>
</ul>
</details>
<li><p><strong>Manipulation</strong>: Sets the arc of the owner figure based on the given x, y coordinates and the anchor x, y coordinates.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invokeStep(int,int,int,int,CH.ifa.draw.framework.DrawingView)</strong>: Set the arc of the owner figure based on the given x, y coordinates and the anchor x, y coordinates.</p></li>
</ul>
</details>
<li><p><strong>Location</strong>: Calculates and returns the location of the radius handle for the figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>locate()</strong>: Calculate and return the location of the radius handle for the figure.</p></li>
</ul>
</details>
<li><p><strong>Manipulation</strong>: Sets the radius of the figure's arc to half of its current value.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invokeStart(int,int,CH.ifa.draw.framework.DrawingView)</strong>: Set the radius of the figure's arc to half of its current value.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.GroupHandle</strong>: Draws a group handle with a black rectangle and white border.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Drawing</strong>: Draws a black rectangle with a white border representing the display box of the group handle.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws a black rectangle with a white border representing the display box of the group handle.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.ElbowHandle</strong>: Draws and manipulates an elbow handle for a line connection.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Drawing</strong>: Draws a yellow filled oval and a black outline oval on the graphics object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws a yellow filled oval and a black outline oval on the graphics object.</p></li>
</ul>
</details>
<li><p><strong>Locating</strong>: Returns the midpoint between two points on a line connection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>locate()</strong>: Return the midpoint between two points on a line connection.</p></li>
</ul>
</details>
<li><p><strong>Updating</strong>: Sets the last known x and y coordinates to the given x and y values.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invokeStart(int,int,CH.ifa.draw.framework.DrawingView)</strong>: Set the last known x and y coordinates to the given x and y values.</p></li>
</ul>
</details>
<li><p><strong>Positioning</strong>: Updates the position of the elbow handle based on the new coordinates and anchor point.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invokeStep(int,int,int,int,CH.ifa.draw.framework.DrawingView)</strong>: Update the position of the elbow handle based on the new coordinates and anchor point.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.FontSizeHandle</strong>: Set font and size of text figure, calculate new font size, and draw a filled oval with a black outline.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Set font and size</strong>: Set the font and size of the text figure's owner to the current font and size.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invokeStart(int,int,CH.ifa.draw.framework.DrawingView)</strong>: Set the font and size of the text figure's owner to the current font and size.</p></li>
</ul>
</details>
<li><p><strong>Calculate new font size</strong>: Set the font size of the text figure to the calculated new size based on the given parameters.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invokeStep(int,int,int,int,CH.ifa.draw.framework.DrawingView)</strong>: Set the font size of the text figure to the calculated new size based on the given parameters.</p></li>
</ul>
</details>
<li><p><strong>Draw filled oval</strong>: Draws a yellow filled oval with a black outline using the given graphics context.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws a yellow filled oval with a black outline using the given graphics context.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.PolyLineHandle</strong>: Represents a handle for a polyline figure.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Setting point in polyline handle</strong>: Set the point at the specified coordinates in the polyline handle.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invokeStep(int,int,int,int,CH.ifa.draw.framework.DrawingView)</strong>: Set the point at the specified coordinates in the polyline handle.</p></li>
</ul>
</details>
<li><p><strong>Setting anchor point of PolyLineHandle</strong>: Set the anchor point of the PolyLineHandle to the specified coordinates.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invokeStart(int,int,CH.ifa.draw.framework.DrawingView)</strong>: Set the anchor point of the PolyLineHandle to the specified coordinates.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Connection</strong>: Managing connections between figures</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.figures.LineConnection</strong>: Represents a line connection between two figures.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Handle management</strong>: Create and return a vector of handles for the LineConnection object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Create and return a vector of handles for the LineConnection object.</p></li>
</ul>
</details>
<li><p><strong>Figure update</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureRequestUpdate(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
<li><p><strong>figureInvalidated(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Invalidate the figure and update the connection when a FigureChangeEvent occurs.</p></li>
<li><p><strong>figureRemoved(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure from the line connection and notify the listener.</p></li>
<li><p><strong>figureRequestRemove(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure associated with the given FigureChangeEvent from the LineConnection.</p></li>
<li><p><strong>figureChanged(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the connection of the line when a figure change event occurs.</p></li>
</ul>
</details>
<li><p><strong>Point manipulation</strong>: Remove, set, insert, and get points of the line connection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>removePointAt(int)</strong>: Remove the point at the specified index and update the layout of the connection.</p></li>
<li><p><strong>setPointAt(java.awt.Point,int)</strong>: Set the point at the specified index to the given point and update the layout of the connection.</p></li>
<li><p><strong>insertPointAt(java.awt.Point,int)</strong>: Inserts a point at the specified index in the line connection and updates the layout of the connection.</p></li>
<li><p><strong>startPoint()</strong>: Return the starting point of the line connection as a new `java.awt.Point` object.</p></li>
<li><p><strong>startPoint(int,int)</strong>: Set the starting point of the line connection to the specified coordinates.</p></li>
<li><p><strong>endPoint()</strong>: Return the end point of the line connection as a new `java.awt.Point` object.</p></li>
<li><p><strong>endPoint(int,int)</strong>: Set the end point of the line connection to the specified coordinates.</p></li>
</ul>
</details>
<li><p><strong>Connection management</strong>: Check, connect, disconnect, and update the start and end connectors of the line connection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectsSame(CH.ifa.draw.framework.ConnectionFigure)</strong>: Check if the given connection figure has the same start and end points as this line connection.</p></li>
<li><p><strong>connectStart(CH.ifa.draw.framework.Connector)</strong>: Connects the start of the line connection to the given connector and adds a figure change listener to the start figure.</p></li>
<li><p><strong>connectEnd(CH.ifa.draw.framework.Connector)</strong>: Connects the end of the line connection to the given connector and adds a figure change listener to the end figure.</p></li>
<li><p><strong>disconnectStart()</strong>: Disconnects the start figure of the line connection and removes the figure change listener.</p></li>
<li><p><strong>disconnectEnd()</strong>: Disconnects the end of the line connection and removes the figure change listener.</p></li>
<li><p><strong>updateConnection()</strong>: Update the connection points of the line connection based on the start and end figures.</p></li>
<li><p><strong>canConnect()</strong>: Check if a line connection can be established.</p></li>
<li><p><strong>canConnect(CH.ifa.draw.framework.Figure,CH.ifa.draw.framework.Figure)</strong>: Check if a connection can be made between two figures.</p></li>
</ul>
</details>
<li><p><strong>Figure retrieval</strong>: Return the owner figures of the start and end points of the line connection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>startFigure()</strong>: Return the owner figure of the start point of the line connection, or null if there is no start point.</p></li>
<li><p><strong>endFigure()</strong>: Return the owner figure of the end point of the line connection, or null if there is no end point.</p></li>
</ul>
</details>
<li><p><strong>Layout management</strong>: Update the layout of the connection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>layoutConnection()</strong>: Update the connection layout.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Read and write the line connection to a StorableInput or StorableOutput object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the input and connects the start and end connectors of the line connection if they are not null, then updates the connection.</p></li>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the start and end points of the line connection to the specified `StorableOutput` object.</p></li>
</ul>
</details>
<li><p><strong>Release resources</strong>: Disconnect the start and end figures of the line connection and remove the figure change listener.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>release()</strong>: Disconnects the start and end figures of the line connection and removes the figure change listener if present.</p></li>
</ul>
</details>
<li><p><strong>Connector retrieval</strong>: Return the start and end connectors of the line connection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>start()</strong>: Return the starting connector of the line connection.</p></li>
<li><p><strong>end()</strong>: Return the end connector of the line connection.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.ConnectedTextTool</strong>: Activate or deactivate the ConnectedTextTool and connect text holder figure to a pressed figure if not already connected.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Activation</strong>: Set the fConnected variable to false to deactivate the tool.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>activate()</strong>: Set the `fConnected` variable to `false` to deactivate the tool.</p></li>
</ul>
</details>
<li><p><strong>Connection</strong>: Connect the text holder figure to a pressed figure if it is not already connected.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseDown(java.awt.event.MouseEvent,int,int)</strong>: Connects the text holder figure to a pressed figure if it is not already connected.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.ElbowConnection</strong>: Update and layout the connection between two figures using elbow connection.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Update connection</strong>: Update the connection of the elbow connection figure by updating its points.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>updateConnection()</strong>: Update the connection of the elbow connection figure by updating its points.</p></li>
</ul>
</details>
<li><p><strong>Layout connection</strong>: Layout the connection between two figures.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>layoutConnection()</strong>: Layout the connection between two figures.</p></li>
</ul>
</details>
<li><p><strong>Get connected text locator</strong>: Return a locator for the connected text of the given figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectedTextLocator(CH.ifa.draw.framework.Figure)</strong>: Return a locator for the connected text of the given figure.</p></li>
</ul>
</details>
<li><p><strong>Create handles</strong>: Create and return a vector of handles for the ElbowConnection figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Create and return a vector of handles for the ElbowConnection figure.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Drawing</strong>: Drawing figures on a canvas</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.figures.PolyLineFigure</strong>: This class represents a polyline figure that can be drawn and manipulated.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Bounding Box</strong>: Calculate and return the bounding box of the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>displayBox()</strong>: Calculate and return the bounding box of the polyline figure.</p></li>
</ul>
</details>
<li><p><strong>Drawing</strong>: Draw the polyline figure by connecting the points and decorating it.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws a polyline figure by connecting the points in the fPoints vector with lines and decorates it.</p></li>
</ul>
</details>
<li><p><strong>Point Manipulation</strong>: Set, get, insert, and remove points in the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setPointAt(java.awt.Point,int)</strong>: Set the point at the specified index to the given point.</p></li>
<li><p><strong>pointAt(int)</strong>: Return the point at the specified index in the PolyLineFigure's list of points.</p></li>
<li><p><strong>addPoint(int,int)</strong>: Add a new point to the polyline figure at the specified coordinates.</p></li>
<li><p><strong>insertPointAt(java.awt.Point,int)</strong>: Inserts a new point at the specified index in the polyline figure.</p></li>
<li><p><strong>removePointAt(int)</strong>: Remove the point at the specified index from the PolyLineFigure.</p></li>
<li><p><strong>pointCount()</strong>: Return the number of points in the PolyLineFigure.</p></li>
</ul>
</details>
<li><p><strong>Empty Check</strong>: Check if the polyline figure is empty.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>isEmpty()</strong>: Check if the PolyLineFigure is empty by determining if its width and height are both less than 3.</p></li>
</ul>
</details>
<li><p><strong>Locator Creation</strong>: Create a locator for a specific point in the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>locator(int)</strong>: Create a locator for the specified point index in the PolyLineFigure.</p></li>
</ul>
</details>
<li><p><strong>Enumeration of Points</strong>: Return an enumeration of the points in the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>points()</strong>: Return an enumeration of the points in the PolyLineFigure.</p></li>
</ul>
</details>
<li><p><strong>Decoration Manipulation</strong>: Set the start and end decorations of the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setStartDecoration(CH.ifa.draw.figures.LineDecoration)</strong>: Set the start decoration of the PolyLineFigure to the specified LineDecoration.</p></li>
<li><p><strong>setEndDecoration(CH.ifa.draw.figures.LineDecoration)</strong>: Set the end decoration of the PolyLineFigure to the specified LineDecoration.</p></li>
</ul>
</details>
<li><p><strong>Point Containment Check</strong>: Check if a given point is contained within the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>containsPoint(int,int)</strong>: Check if the given point is contained within the polyline figure.</p></li>
</ul>
</details>
<li><p><strong>Segment Manipulation</strong>: Join or split segments of the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>joinSegments(int,int)</strong>: Remove a point from the polyline figure if the distance between the given coordinates and the point is less than 3, and return true if a point was removed, otherwise return false.</p></li>
<li><p><strong>splitSegment(int,int)</strong>: Inserts a new point at the specified coordinates in the polyline figure, splitting the segment at the given position.</p></li>
</ul>
</details>
<li><p><strong>Handle Creation</strong>: Create handles for each point in the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Create and return a vector of handles for each point in the PolyLineFigure.</p></li>
</ul>
</details>
<li><p><strong>Attribute Manipulation</strong>: Set and get attributes of the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setAttribute(java.lang.String,java.lang.Object)</strong>: Set the specified attribute of the PolyLineFigure.</p></li>
<li><p><strong>getAttribute(java.lang.String)</strong>: Return the value of the specified attribute for the PolyLineFigure.</p></li>
</ul>
</details>
<li><p><strong>Segment Finding</strong>: Find the segment of the polyline figure that contains a given point.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>findSegment(int,int)</strong>: Find the segment of the polyline figure that contains the given coordinates.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Read and write the state of the polyline figure to a stream.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the state of a PolyLineFigure object from a StorableInput object.</p></li>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the PolyLineFigure object to the StorableOutput stream, including its points, decorations, and frame color.</p></li>
</ul>
</details>
<li><p><strong>Display Box Setting</strong>: Set the display box of the polyline figure using given origin and corner points.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Set the display box of the PolyLineFigure using the given origin and corner points.</p></li>
</ul>
</details>
<li><p><strong>Connector Retrieval</strong>: Return a connector at a specific coordinates for the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectorAt(int,int)</strong>: Return a connector at the specified coordinates for the PolyLineFigure.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.LineFigure</strong>: Represents a line figure in a drawing.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Get end point</strong>: Return the end point of the line figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>endPoint()</strong>: Return the end point of the line figure.</p></li>
</ul>
</details>
<li><p><strong>Set origin and corner points</strong>: Set the origin and corner points of the line figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Set the origin and corner points of the line figure.</p></li>
</ul>
</details>
<li><p><strong>Get starting point</strong>: Return the starting point of the line figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>startPoint()</strong>: Return the starting point of the line figure.</p></li>
</ul>
</details>
<li><p><strong>Set starting point</strong>: Set the starting point of the line figure to the specified coordinates.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>startPoint(int,int)</strong>: Set the starting point of the line figure to the specified coordinates.</p></li>
</ul>
</details>
<li><p><strong>Set endpoint</strong>: Set the endpoint of the line figure to the specified coordinates.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>endPoint(int,int)</strong>: Set the endpoint of the line figure to the specified coordinates.</p></li>
</ul>
</details>
<li><p><strong>Set start and end points</strong>: Set the start and end points of the line figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setPoints(java.awt.Point,java.awt.Point)</strong>: Set the start and end points of the line figure.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.EllipseFigure</strong>: Represents an ellipse figure that can be displayed and manipulated in a drawing application.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Handle management</strong>: Add handles to the ellipse figure and return them as a vector.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Add handles to the ellipse figure and return them as a vector.</p></li>
</ul>
</details>
<li><p><strong>Connector management</strong>: Return a connector at the specified coordinates on the ellipse figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectorAt(int,int)</strong>: Return a connector at the specified coordinates on the ellipse figure.</p></li>
</ul>
</details>
<li><p><strong>Display box management</strong>: Return the display box of the ellipse figure as a new rectangle.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>displayBox()</strong>: Return the display box of the ellipse figure as a new rectangle.</p></li>
</ul>
</details>
<li><p><strong>Drawing</strong>: Draws the frame of the ellipse figure using the given graphics object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawFrame(java.awt.Graphics)</strong>: Draws the frame of the ellipse figure using the given graphics object.</p></li>
</ul>
</details>
<li><p><strong>Connection management</strong>: Return the insets for connections to this ellipse figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectionInsets()</strong>: Return the insets for connections to this ellipse figure.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Reads the state of the EllipseFigure object from the given StorableInput and sets the display box accordingly.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the state of the `EllipseFigure` object from the given `StorableInput` and sets the display box accordingly.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Write the display box coordinates and dimensions of the ellipse figure to the specified storable output.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the display box coordinates and dimensions of the ellipse figure to the specified storable output.</p></li>
</ul>
</details>
<li><p><strong>Drawing</strong>: Draws the background of the ellipse figure by filling the oval shape with the specified graphics context.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawBackground(java.awt.Graphics)</strong>: Draws the background of the ellipse figure by filling the oval shape with the specified graphics context.</p></li>
</ul>
</details>
<li><p><strong>Display box management</strong>: Set the display box of the ellipse figure based on the given origin and corner points.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Set the display box of the ellipse figure based on the given origin and corner points.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.BorderDecorator</strong>: Calculate and display the display box of the BorderDecorator figure with specified border dimensions, update the invalidated rectangle of the figure, adjust the connection insets, and draw a border around the figure with white and gray lines.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Calculate and display display box</strong>: Calculate and return the display box of the BorderDecorator figure by growing the component's display box by the specified border dimensions.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>displayBox()</strong>: Calculate and return the display box of the BorderDecorator figure by growing the component's display box by the specified border dimensions.</p></li>
</ul>
</details>
<li><p><strong>Update invalidated rectangle</strong>: Update the invalidated rectangle of the figure with the border dimensions and notify the superclass about the figure change event.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureInvalidated(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the invalidated rectangle of the figure with the border dimensions and notify the superclass about the figure change event.</p></li>
</ul>
</details>
<li><p><strong>Adjust connection insets</strong>: Adjusts the connection insets of the figure by subtracting 3 from the top, bottom, left, and right insets.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectionInsets()</strong>: Adjusts the connection insets of the figure by subtracting 3 from the top, bottom, left, and right insets.</p></li>
</ul>
</details>
<li><p><strong>Draw border</strong>: Draws a border around the figure with white and gray lines.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws a border around the figure with white and gray lines.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.RectangleFigure</strong>: This class represents a rectangle figure and provides methods for drawing, manipulating, and storing the figure.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Drawing</strong>: Draws the frame and background of the rectangle figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawFrame(java.awt.Graphics)</strong>: Draws the frame of the rectangle figure using the given graphics object.</p></li>
<li><p><strong>drawBackground(java.awt.Graphics)</strong>: Draws the background of the rectangle figure using the given graphics object.</p></li>
</ul>
</details>
<li><p><strong>Manipulating</strong>: Sets the display box of the rectangle figure and returns its coordinates and dimensions.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Set the display box of the rectangle figure using the given origin and corner points.</p></li>
<li><p><strong>displayBox()</strong>: Return the display box of the rectangle figure as a new instance of java.awt.Rectangle.</p></li>
</ul>
</details>
<li><p><strong>Storing</strong>: Reads and writes the state of the rectangle figure to a storable input/output.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the state of the RectangleFigure object from the given StorableInput.</p></li>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the display box coordinates and dimensions of the rectangle figure to the specified storable output.</p></li>
</ul>
</details>
<li><p><strong>Handling</strong>: Adds handles to the rectangle figure and returns them as a vector.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Add handles to the rectangle figure and return them as a vector.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.ArrowTip</strong>: Represents an arrow tip that can be drawn and saved to a StorableOutput.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Saving to StorableOutput</strong>: Save the ArrowTip object to a StorableOutput.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the method `write(CH.ifa.draw.util.StorableOutput)` to save the ArrowTip object to a StorableOutput.</p></li>
</ul>
</details>
<li><p><strong>Drawing</strong>: Draw an arrow tip at specified coordinates using a graphics object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics,int,int,int,int)</strong>: Draws an arrow tip at the specified coordinates using the given graphics object.</p></li>
</ul>
</details>
<li><p><strong>Reading from StorableInput</strong>: Read the state of the ArrowTip object from a StorableInput.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the state of the ArrowTip object from the given StorableInput.</p></li>
</ul>
</details>
<li><p><strong>Calculating outline</strong>: Calculate the outline of an arrow tip given the coordinates of two points.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>outline(int,int,int,int)</strong>: Calculate the outline of an arrow tip given the coordinates of two points.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>abstract class <strong>CH.ifa.draw.figures.AttributeFigure</strong>: Represents an attribute figure that can be drawn with specified fill and frame colors and can have attributes with default values.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Color Management</strong>: Manage the frame and fill colors of the attribute figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getFrameColor()</strong>: Return the frame color of the attribute figure.</p></li>
<li><p><strong>getFillColor()</strong>: Return the fill color of the attribute figure.</p></li>
</ul>
</details>
<li><p><strong>Attribute Management</strong>: Manage the attributes of the figure, including getting the default value, getting the value, setting the value, and notifying observers of changes.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getDefaultAttribute(java.lang.String)</strong>: Return the default attribute value for the given name.</p></li>
<li><p><strong>getAttribute(java.lang.String)</strong>: Return the value of the specified attribute if it is defined, otherwise return the default attribute value.</p></li>
<li><p><strong>setAttribute(java.lang.String,java.lang.Object)</strong>: Set the specified attribute to the given value and notify any observers of the change.</p></li>
</ul>
</details>
<li><p><strong>Drawing</strong>: Draw the figure with the specified fill and frame colors.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws the figure with the specified fill color and frame color.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Read and write the attributes of the figure to a stream.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the attributes of the figure to the given `StorableOutput` object.</p></li>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the attributes of a figure from the given input stream.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.ImageFigure</strong>: Draws and manages an image figure.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Drawing</strong>: Draws the image on the graphics object if it exists, otherwise draws a ghost image.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws the image on the graphics object if it exists, otherwise draws a ghost image.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Reads and writes the state of an ImageFigure object from/to a StorableInput/StorableOutput object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the state of an ImageFigure object from a StorableInput object, including its display box, file name, and registers the image with the Iconkit.</p></li>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the display box coordinates and file name of the image figure to the specified storable output.</p></li>
</ul>
</details>
<li><p><strong>Image Management</strong>: Updates the image and notifies the listener if the image has changed.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>imageUpdate(java.awt.Image,int,int,int,int,int)</strong>: Update the image and notify the listener if the image has changed.</p></li>
</ul>
</details>
<li><p><strong>Handle Management</strong>: Adds handles to the image figure and returns them as a vector.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Add handles to the image figure and return them as a vector.</p></li>
</ul>
</details>
<li><p><strong>Display Box Management</strong>: Sets and returns the display box of the image figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Set the display box of the image figure based on the given origin and corner points.</p></li>
<li><p><strong>displayBox()</strong>: Return the display box of the image figure as a new rectangle.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.RoundRectangleFigure</strong>: Represents a round rectangle figure.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Connection handling</strong>: Return the insets for connections to this round rectangle figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectionInsets()</strong>: Return the insets for connections to this round rectangle figure.</p></li>
</ul>
</details>
<li><p><strong>Connector handling</strong>: Return the connector at the specified coordinates in the RoundRectangleFigure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectorAt(int,int)</strong>: Return the connector at the specified coordinates in the RoundRectangleFigure.</p></li>
</ul>
</details>
<li><p><strong>Arc handling</strong>: Set the width and height of the arc of the round rectangle figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setArc(int,int)</strong>: Set the width and height of the arc of the round rectangle figure.</p></li>
<li><p><strong>getArc()</strong>: Return the arc width and height of the round rectangle figure as a Point object.</p></li>
</ul>
</details>
<li><p><strong>Display box handling</strong>: Return the display box of the round rectangle figure as a new rectangle object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>displayBox()</strong>: Return the display box of the round rectangle figure as a new rectangle object.</p></li>
</ul>
</details>
<li><p><strong>Frame handling</strong>: Draws the frame of the round rectangle figure using the given graphics object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawFrame(java.awt.Graphics)</strong>: Draws the frame of the round rectangle figure using the given graphics object.</p></li>
</ul>
</details>
<li><p><strong>Serialization handling</strong>: Write the state of the RoundRectangleFigure object to the StorableOutput stream.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the state of the RoundRectangleFigure object to the StorableOutput stream.</p></li>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the state of a RoundRectangleFigure object from the given StorableInput.</p></li>
</ul>
</details>
<li><p><strong>Display box manipulation</strong>: Set the display box of the round rectangle figure based on the given origin and corner points.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Set the display box of the round rectangle figure based on the given origin and corner points.</p></li>
</ul>
</details>
<li><p><strong>Handle handling</strong>: Add handles to the round rectangle figure and include a radius handle.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Add handles to the round rectangle figure and include a radius handle.</p></li>
</ul>
</details>
<li><p><strong>Background handling</strong>: Draws the background of the round rectangle figure using the specified graphics context.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawBackground(java.awt.Graphics)</strong>: Draws the background of the round rectangle figure using the specified graphics context.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.TextFigure</strong>: Represents a text figure that can be displayed and manipulated in a drawing.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Figure Change</strong>: Update the location of the text figure when a figure change event occurs.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureChanged(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the location of the text figure when a figure change event occurs.</p></li>
</ul>
</details>
<li><p><strong>Read-only</strong>: Manage the read-only state of the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>readOnly()</strong>: Return whether the text figure is read-only or not.</p></li>
<li><p><strong>setReadOnly(boolean)</strong>: Set the read-only state of the text figure.</p></li>
</ul>
</details>
<li><p><strong>Text Manipulation</strong>: Get and set the text of the TextFigure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getText()</strong>: Return the text of the TextFigure.</p></li>
<li><p><strong>setText(java.lang.String)</strong>: Set the text of the TextFigure to the specified new text.</p></li>
</ul>
</details>
<li><p><strong>Figure Connection</strong>: Connect and disconnect the text figure to/from other figures.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connect(CH.ifa.draw.framework.Figure)</strong>: Connects the text figure to a given figure and updates its location.</p></li>
<li><p><strong>disconnect()</strong>: Disconnects the observed figure and sets the observed figure and locator to null.</p></li>
</ul>
</details>
<li><p><strong>Font Manipulation</strong>: Manage the font used by the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setFont(java.awt.Font)</strong>: Set the font of the text figure to the specified font.</p></li>
<li><p><strong>setCurrentFontStyle(int)</strong>: Set the current font style for the TextFigure class.</p></li>
<li><p><strong>setCurrentFontName(java.lang.String)</strong>: Set the current font name to the specified name.</p></li>
<li><p><strong>setCurrentFontSize(int)</strong>: Set the current font size to the specified size.</p></li>
<li><p><strong>createCurrentFont()</strong>: Create and return a new `java.awt.Font` object using the current font name, style, and size.</p></li>
</ul>
</details>
<li><p><strong>Figure Removal</strong>: Remove a figure from the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureRequestRemove(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure specified in the FigureChangeEvent from the TextFigure.</p></li>
<li><p><strong>figureRemoved(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure from the listener if it exists.</p></li>
</ul>
</details>
<li><p><strong>Figure Display</strong>: Manage the display of the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>displayBox()</strong>: Return the bounding box of the text figure.</p></li>
<li><p><strong>overlayColumns()</strong>: Calculate the number of columns needed to overlay the text in the figure.</p></li>
<li><p><strong>handles()</strong>: Create and return a vector of handles for the TextFigure object.</p></li>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Set the origin of the text figure to the specified point.</p></li>
<li><p><strong>drawBackground(java.awt.Graphics)</strong>: Draws the background of the text figure using the given graphics object.</p></li>
<li><p><strong>drawFrame(java.awt.Graphics)</strong>: Draws the text figure's frame using the specified graphics context.</p></li>
<li><p><strong>textDisplayBox()</strong>: Return the bounding rectangle that encloses the text displayed by this TextFigure.</p></li>
</ul>
</details>
<li><p><strong>Figure Update</strong>: Update the figure based on a change event.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureRequestUpdate(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
<li><p><strong>figureInvalidated(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Invalidate the figure when a change event occurs.</p></li>
</ul>
</details>
<li><p><strong>Resource Management</strong>: Release resources held by the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>release()</strong>: Release any resources held by the TextFigure and remove it as an observer of any observed figures.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Read and write the state of the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the state of the TextFigure object to the StorableOutput stream.</p></li>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the state of a TextFigure object from a StorableInput object, including its origin, text, font, read-only status, observed figure, and locator.</p></li>
</ul>
</details>
<li><p><strong>Attribute Manipulation</strong>: Manage the attributes of the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setAttribute(java.lang.String,java.lang.Object)</strong>: Set the specified attribute of the TextFigure, such as font size, style, or name.</p></li>
<li><p><strong>getAttribute(java.lang.String)</strong>: Return the value of the specified attribute for the TextFigure.</p></li>
</ul>
</details>
<li><p><strong>Typing Acceptance</strong>: Check if the text figure can accept typing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>acceptsTyping()</strong>: Check if the text figure is not read-only and can accept typing.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Serialization</strong>: Serializing and deserializing figures</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.figures.FigureAttributes</strong>: Represents the attributes of a figure and provides methods to manipulate and retrieve these attributes.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Attribute Manipulation</strong>: Methods to set, get, and check the existence of attributes in the FigureAttributes map.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>set(java.lang.String,java.lang.Object)</strong>: Set the value of the specified attribute with the given name.</p></li>
<li><p><strong>get(java.lang.String)</strong>: Return the value associated with the specified name from the map.</p></li>
<li><p><strong>hasDefined(java.lang.String)</strong>: Check if the specified name is defined in the FigureAttributes map.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Methods to write and read the attributes of a figure to/from a StorableOutput/StorableInput object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the attributes of the figure to the given StorableOutput object.</p></li>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the attributes of a figure from a StorableInput object and stores them in a Hashtable.</p></li>
</ul>
</details>
<li><p><strong>Cloning</strong>: Method to create a clone of the FigureAttributes object and its associated Hashtable.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>clone()</strong>: Clone the FigureAttributes object and its associated Hashtable, and return the cloned object.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.PolyLineFigure</strong>: This class represents a polyline figure that can be drawn and manipulated.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Bounding Box</strong>: Calculate and return the bounding box of the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>displayBox()</strong>: Calculate and return the bounding box of the polyline figure.</p></li>
</ul>
</details>
<li><p><strong>Drawing</strong>: Draw the polyline figure by connecting the points and decorating it.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws a polyline figure by connecting the points in the fPoints vector with lines and decorates it.</p></li>
</ul>
</details>
<li><p><strong>Point Manipulation</strong>: Set, get, insert, and remove points in the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setPointAt(java.awt.Point,int)</strong>: Set the point at the specified index to the given point.</p></li>
<li><p><strong>pointAt(int)</strong>: Return the point at the specified index in the PolyLineFigure's list of points.</p></li>
<li><p><strong>addPoint(int,int)</strong>: Add a new point to the polyline figure at the specified coordinates.</p></li>
<li><p><strong>insertPointAt(java.awt.Point,int)</strong>: Inserts a new point at the specified index in the polyline figure.</p></li>
<li><p><strong>removePointAt(int)</strong>: Remove the point at the specified index from the PolyLineFigure.</p></li>
<li><p><strong>pointCount()</strong>: Return the number of points in the PolyLineFigure.</p></li>
</ul>
</details>
<li><p><strong>Empty Check</strong>: Check if the polyline figure is empty.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>isEmpty()</strong>: Check if the PolyLineFigure is empty by determining if its width and height are both less than 3.</p></li>
</ul>
</details>
<li><p><strong>Locator Creation</strong>: Create a locator for a specific point in the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>locator(int)</strong>: Create a locator for the specified point index in the PolyLineFigure.</p></li>
</ul>
</details>
<li><p><strong>Enumeration of Points</strong>: Return an enumeration of the points in the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>points()</strong>: Return an enumeration of the points in the PolyLineFigure.</p></li>
</ul>
</details>
<li><p><strong>Decoration Manipulation</strong>: Set the start and end decorations of the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setStartDecoration(CH.ifa.draw.figures.LineDecoration)</strong>: Set the start decoration of the PolyLineFigure to the specified LineDecoration.</p></li>
<li><p><strong>setEndDecoration(CH.ifa.draw.figures.LineDecoration)</strong>: Set the end decoration of the PolyLineFigure to the specified LineDecoration.</p></li>
</ul>
</details>
<li><p><strong>Point Containment Check</strong>: Check if a given point is contained within the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>containsPoint(int,int)</strong>: Check if the given point is contained within the polyline figure.</p></li>
</ul>
</details>
<li><p><strong>Segment Manipulation</strong>: Join or split segments of the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>joinSegments(int,int)</strong>: Remove a point from the polyline figure if the distance between the given coordinates and the point is less than 3, and return true if a point was removed, otherwise return false.</p></li>
<li><p><strong>splitSegment(int,int)</strong>: Inserts a new point at the specified coordinates in the polyline figure, splitting the segment at the given position.</p></li>
</ul>
</details>
<li><p><strong>Handle Creation</strong>: Create handles for each point in the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Create and return a vector of handles for each point in the PolyLineFigure.</p></li>
</ul>
</details>
<li><p><strong>Attribute Manipulation</strong>: Set and get attributes of the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setAttribute(java.lang.String,java.lang.Object)</strong>: Set the specified attribute of the PolyLineFigure.</p></li>
<li><p><strong>getAttribute(java.lang.String)</strong>: Return the value of the specified attribute for the PolyLineFigure.</p></li>
</ul>
</details>
<li><p><strong>Segment Finding</strong>: Find the segment of the polyline figure that contains a given point.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>findSegment(int,int)</strong>: Find the segment of the polyline figure that contains the given coordinates.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Read and write the state of the polyline figure to a stream.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the state of a PolyLineFigure object from a StorableInput object.</p></li>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the PolyLineFigure object to the StorableOutput stream, including its points, decorations, and frame color.</p></li>
</ul>
</details>
<li><p><strong>Display Box Setting</strong>: Set the display box of the polyline figure using given origin and corner points.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Set the display box of the PolyLineFigure using the given origin and corner points.</p></li>
</ul>
</details>
<li><p><strong>Connector Retrieval</strong>: Return a connector at a specific coordinates for the polyline figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectorAt(int,int)</strong>: Return a connector at the specified coordinates for the PolyLineFigure.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.LineConnection</strong>: Represents a line connection between two figures.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Handle management</strong>: Create and return a vector of handles for the LineConnection object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Create and return a vector of handles for the LineConnection object.</p></li>
</ul>
</details>
<li><p><strong>Figure update</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureRequestUpdate(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
<li><p><strong>figureInvalidated(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Invalidate the figure and update the connection when a FigureChangeEvent occurs.</p></li>
<li><p><strong>figureRemoved(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure from the line connection and notify the listener.</p></li>
<li><p><strong>figureRequestRemove(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure associated with the given FigureChangeEvent from the LineConnection.</p></li>
<li><p><strong>figureChanged(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the connection of the line when a figure change event occurs.</p></li>
</ul>
</details>
<li><p><strong>Point manipulation</strong>: Remove, set, insert, and get points of the line connection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>removePointAt(int)</strong>: Remove the point at the specified index and update the layout of the connection.</p></li>
<li><p><strong>setPointAt(java.awt.Point,int)</strong>: Set the point at the specified index to the given point and update the layout of the connection.</p></li>
<li><p><strong>insertPointAt(java.awt.Point,int)</strong>: Inserts a point at the specified index in the line connection and updates the layout of the connection.</p></li>
<li><p><strong>startPoint()</strong>: Return the starting point of the line connection as a new `java.awt.Point` object.</p></li>
<li><p><strong>startPoint(int,int)</strong>: Set the starting point of the line connection to the specified coordinates.</p></li>
<li><p><strong>endPoint()</strong>: Return the end point of the line connection as a new `java.awt.Point` object.</p></li>
<li><p><strong>endPoint(int,int)</strong>: Set the end point of the line connection to the specified coordinates.</p></li>
</ul>
</details>
<li><p><strong>Connection management</strong>: Check, connect, disconnect, and update the start and end connectors of the line connection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectsSame(CH.ifa.draw.framework.ConnectionFigure)</strong>: Check if the given connection figure has the same start and end points as this line connection.</p></li>
<li><p><strong>connectStart(CH.ifa.draw.framework.Connector)</strong>: Connects the start of the line connection to the given connector and adds a figure change listener to the start figure.</p></li>
<li><p><strong>connectEnd(CH.ifa.draw.framework.Connector)</strong>: Connects the end of the line connection to the given connector and adds a figure change listener to the end figure.</p></li>
<li><p><strong>disconnectStart()</strong>: Disconnects the start figure of the line connection and removes the figure change listener.</p></li>
<li><p><strong>disconnectEnd()</strong>: Disconnects the end of the line connection and removes the figure change listener.</p></li>
<li><p><strong>updateConnection()</strong>: Update the connection points of the line connection based on the start and end figures.</p></li>
<li><p><strong>canConnect()</strong>: Check if a line connection can be established.</p></li>
<li><p><strong>canConnect(CH.ifa.draw.framework.Figure,CH.ifa.draw.framework.Figure)</strong>: Check if a connection can be made between two figures.</p></li>
</ul>
</details>
<li><p><strong>Figure retrieval</strong>: Return the owner figures of the start and end points of the line connection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>startFigure()</strong>: Return the owner figure of the start point of the line connection, or null if there is no start point.</p></li>
<li><p><strong>endFigure()</strong>: Return the owner figure of the end point of the line connection, or null if there is no end point.</p></li>
</ul>
</details>
<li><p><strong>Layout management</strong>: Update the layout of the connection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>layoutConnection()</strong>: Update the connection layout.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Read and write the line connection to a StorableInput or StorableOutput object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the input and connects the start and end connectors of the line connection if they are not null, then updates the connection.</p></li>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the start and end points of the line connection to the specified `StorableOutput` object.</p></li>
</ul>
</details>
<li><p><strong>Release resources</strong>: Disconnect the start and end figures of the line connection and remove the figure change listener.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>release()</strong>: Disconnects the start and end figures of the line connection and removes the figure change listener if present.</p></li>
</ul>
</details>
<li><p><strong>Connector retrieval</strong>: Return the start and end connectors of the line connection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>start()</strong>: Return the starting connector of the line connection.</p></li>
<li><p><strong>end()</strong>: Return the end connector of the line connection.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.ImageFigure</strong>: Draws and manages an image figure.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Drawing</strong>: Draws the image on the graphics object if it exists, otherwise draws a ghost image.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws the image on the graphics object if it exists, otherwise draws a ghost image.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Reads and writes the state of an ImageFigure object from/to a StorableInput/StorableOutput object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the state of an ImageFigure object from a StorableInput object, including its display box, file name, and registers the image with the Iconkit.</p></li>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the display box coordinates and file name of the image figure to the specified storable output.</p></li>
</ul>
</details>
<li><p><strong>Image Management</strong>: Updates the image and notifies the listener if the image has changed.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>imageUpdate(java.awt.Image,int,int,int,int,int)</strong>: Update the image and notify the listener if the image has changed.</p></li>
</ul>
</details>
<li><p><strong>Handle Management</strong>: Adds handles to the image figure and returns them as a vector.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Add handles to the image figure and return them as a vector.</p></li>
</ul>
</details>
<li><p><strong>Display Box Management</strong>: Sets and returns the display box of the image figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Set the display box of the image figure based on the given origin and corner points.</p></li>
<li><p><strong>displayBox()</strong>: Return the display box of the image figure as a new rectangle.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.TextFigure</strong>: Represents a text figure that can be displayed and manipulated in a drawing.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Figure Change</strong>: Update the location of the text figure when a figure change event occurs.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureChanged(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the location of the text figure when a figure change event occurs.</p></li>
</ul>
</details>
<li><p><strong>Read-only</strong>: Manage the read-only state of the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>readOnly()</strong>: Return whether the text figure is read-only or not.</p></li>
<li><p><strong>setReadOnly(boolean)</strong>: Set the read-only state of the text figure.</p></li>
</ul>
</details>
<li><p><strong>Text Manipulation</strong>: Get and set the text of the TextFigure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getText()</strong>: Return the text of the TextFigure.</p></li>
<li><p><strong>setText(java.lang.String)</strong>: Set the text of the TextFigure to the specified new text.</p></li>
</ul>
</details>
<li><p><strong>Figure Connection</strong>: Connect and disconnect the text figure to/from other figures.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connect(CH.ifa.draw.framework.Figure)</strong>: Connects the text figure to a given figure and updates its location.</p></li>
<li><p><strong>disconnect()</strong>: Disconnects the observed figure and sets the observed figure and locator to null.</p></li>
</ul>
</details>
<li><p><strong>Font Manipulation</strong>: Manage the font used by the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setFont(java.awt.Font)</strong>: Set the font of the text figure to the specified font.</p></li>
<li><p><strong>setCurrentFontStyle(int)</strong>: Set the current font style for the TextFigure class.</p></li>
<li><p><strong>setCurrentFontName(java.lang.String)</strong>: Set the current font name to the specified name.</p></li>
<li><p><strong>setCurrentFontSize(int)</strong>: Set the current font size to the specified size.</p></li>
<li><p><strong>createCurrentFont()</strong>: Create and return a new `java.awt.Font` object using the current font name, style, and size.</p></li>
</ul>
</details>
<li><p><strong>Figure Removal</strong>: Remove a figure from the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureRequestRemove(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure specified in the FigureChangeEvent from the TextFigure.</p></li>
<li><p><strong>figureRemoved(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure from the listener if it exists.</p></li>
</ul>
</details>
<li><p><strong>Figure Display</strong>: Manage the display of the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>displayBox()</strong>: Return the bounding box of the text figure.</p></li>
<li><p><strong>overlayColumns()</strong>: Calculate the number of columns needed to overlay the text in the figure.</p></li>
<li><p><strong>handles()</strong>: Create and return a vector of handles for the TextFigure object.</p></li>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Set the origin of the text figure to the specified point.</p></li>
<li><p><strong>drawBackground(java.awt.Graphics)</strong>: Draws the background of the text figure using the given graphics object.</p></li>
<li><p><strong>drawFrame(java.awt.Graphics)</strong>: Draws the text figure's frame using the specified graphics context.</p></li>
<li><p><strong>textDisplayBox()</strong>: Return the bounding rectangle that encloses the text displayed by this TextFigure.</p></li>
</ul>
</details>
<li><p><strong>Figure Update</strong>: Update the figure based on a change event.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureRequestUpdate(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
<li><p><strong>figureInvalidated(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Invalidate the figure when a change event occurs.</p></li>
</ul>
</details>
<li><p><strong>Resource Management</strong>: Release resources held by the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>release()</strong>: Release any resources held by the TextFigure and remove it as an observer of any observed figures.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Read and write the state of the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the state of the TextFigure object to the StorableOutput stream.</p></li>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the state of a TextFigure object from a StorableInput object, including its origin, text, font, read-only status, observed figure, and locator.</p></li>
</ul>
</details>
<li><p><strong>Attribute Manipulation</strong>: Manage the attributes of the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setAttribute(java.lang.String,java.lang.Object)</strong>: Set the specified attribute of the TextFigure, such as font size, style, or name.</p></li>
<li><p><strong>getAttribute(java.lang.String)</strong>: Return the value of the specified attribute for the TextFigure.</p></li>
</ul>
</details>
<li><p><strong>Typing Acceptance</strong>: Check if the text figure can accept typing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>acceptsTyping()</strong>: Check if the text figure is not read-only and can accept typing.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Layout</strong>: Managing the layout of figures</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.figures.LineConnection</strong>: Represents a line connection between two figures.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Handle management</strong>: Create and return a vector of handles for the LineConnection object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Create and return a vector of handles for the LineConnection object.</p></li>
</ul>
</details>
<li><p><strong>Figure update</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureRequestUpdate(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
<li><p><strong>figureInvalidated(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Invalidate the figure and update the connection when a FigureChangeEvent occurs.</p></li>
<li><p><strong>figureRemoved(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure from the line connection and notify the listener.</p></li>
<li><p><strong>figureRequestRemove(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure associated with the given FigureChangeEvent from the LineConnection.</p></li>
<li><p><strong>figureChanged(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the connection of the line when a figure change event occurs.</p></li>
</ul>
</details>
<li><p><strong>Point manipulation</strong>: Remove, set, insert, and get points of the line connection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>removePointAt(int)</strong>: Remove the point at the specified index and update the layout of the connection.</p></li>
<li><p><strong>setPointAt(java.awt.Point,int)</strong>: Set the point at the specified index to the given point and update the layout of the connection.</p></li>
<li><p><strong>insertPointAt(java.awt.Point,int)</strong>: Inserts a point at the specified index in the line connection and updates the layout of the connection.</p></li>
<li><p><strong>startPoint()</strong>: Return the starting point of the line connection as a new `java.awt.Point` object.</p></li>
<li><p><strong>startPoint(int,int)</strong>: Set the starting point of the line connection to the specified coordinates.</p></li>
<li><p><strong>endPoint()</strong>: Return the end point of the line connection as a new `java.awt.Point` object.</p></li>
<li><p><strong>endPoint(int,int)</strong>: Set the end point of the line connection to the specified coordinates.</p></li>
</ul>
</details>
<li><p><strong>Connection management</strong>: Check, connect, disconnect, and update the start and end connectors of the line connection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectsSame(CH.ifa.draw.framework.ConnectionFigure)</strong>: Check if the given connection figure has the same start and end points as this line connection.</p></li>
<li><p><strong>connectStart(CH.ifa.draw.framework.Connector)</strong>: Connects the start of the line connection to the given connector and adds a figure change listener to the start figure.</p></li>
<li><p><strong>connectEnd(CH.ifa.draw.framework.Connector)</strong>: Connects the end of the line connection to the given connector and adds a figure change listener to the end figure.</p></li>
<li><p><strong>disconnectStart()</strong>: Disconnects the start figure of the line connection and removes the figure change listener.</p></li>
<li><p><strong>disconnectEnd()</strong>: Disconnects the end of the line connection and removes the figure change listener.</p></li>
<li><p><strong>updateConnection()</strong>: Update the connection points of the line connection based on the start and end figures.</p></li>
<li><p><strong>canConnect()</strong>: Check if a line connection can be established.</p></li>
<li><p><strong>canConnect(CH.ifa.draw.framework.Figure,CH.ifa.draw.framework.Figure)</strong>: Check if a connection can be made between two figures.</p></li>
</ul>
</details>
<li><p><strong>Figure retrieval</strong>: Return the owner figures of the start and end points of the line connection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>startFigure()</strong>: Return the owner figure of the start point of the line connection, or null if there is no start point.</p></li>
<li><p><strong>endFigure()</strong>: Return the owner figure of the end point of the line connection, or null if there is no end point.</p></li>
</ul>
</details>
<li><p><strong>Layout management</strong>: Update the layout of the connection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>layoutConnection()</strong>: Update the connection layout.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Read and write the line connection to a StorableInput or StorableOutput object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the input and connects the start and end connectors of the line connection if they are not null, then updates the connection.</p></li>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the start and end points of the line connection to the specified `StorableOutput` object.</p></li>
</ul>
</details>
<li><p><strong>Release resources</strong>: Disconnect the start and end figures of the line connection and remove the figure change listener.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>release()</strong>: Disconnects the start and end figures of the line connection and removes the figure change listener if present.</p></li>
</ul>
</details>
<li><p><strong>Connector retrieval</strong>: Return the start and end connectors of the line connection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>start()</strong>: Return the starting connector of the line connection.</p></li>
<li><p><strong>end()</strong>: Return the end connector of the line connection.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.ElbowConnection</strong>: Update and layout the connection between two figures using elbow connection.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Update connection</strong>: Update the connection of the elbow connection figure by updating its points.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>updateConnection()</strong>: Update the connection of the elbow connection figure by updating its points.</p></li>
</ul>
</details>
<li><p><strong>Layout connection</strong>: Layout the connection between two figures.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>layoutConnection()</strong>: Layout the connection between two figures.</p></li>
</ul>
</details>
<li><p><strong>Get connected text locator</strong>: Return a locator for the connected text of the given figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectedTextLocator(CH.ifa.draw.framework.Figure)</strong>: Return a locator for the connected text of the given figure.</p></li>
</ul>
</details>
<li><p><strong>Create handles</strong>: Create and return a vector of handles for the ElbowConnection figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Create and return a vector of handles for the ElbowConnection figure.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Grouping</strong>: Grouping and ungrouping figures</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.figures.GroupHandle</strong>: Draws a group handle with a black rectangle and white border.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Drawing</strong>: Draws a black rectangle with a white border representing the display box of the group handle.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws a black rectangle with a white border representing the display box of the group handle.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.GroupCommand</strong>: Execute group command and check if it is executable.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Execute group command</strong>: Create a new group figure with the selected figures and add it to the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>execute()</strong>: Execute the group command by creating a new group figure with the selected figures and adding it to the drawing.</p></li>
</ul>
</details>
<li><p><strong>Check if command is executable</strong>: Check if there is at least one selected figure in the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>isExecutable()</strong>: Check if there is at least one selected figure in the view.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.GroupFigure</strong>: Set and manipulate a group of figures.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Display Box</strong>: Set and calculate the display box of the GroupFigure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Set the display box of the GroupFigure using the given origin and corner points.</p></li>
<li><p><strong>displayBox()</strong>: Calculate and return the bounding box that encloses all the figures in the group.</p></li>
</ul>
</details>
<li><p><strong>Handles</strong>: Create and return handles for the group figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Create and return a vector of handles for the group figure.</p></li>
</ul>
</details>
<li><p><strong>Decompose</strong>: Decompose the group figure into individual figures.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>decompose()</strong>: Decomposes the group figure into individual figures and returns an enumeration of them.</p></li>
</ul>
</details>
<li><p><strong>Attribute</strong>: Set attributes for the GroupFigure and its contained figures.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setAttribute(java.lang.String,java.lang.Object)</strong>: Set the specified attribute with the given value for the GroupFigure and all its contained figures.</p></li>
</ul>
</details>
<li><p><strong>Connectivity</strong>: Check if the figure can be connected to other figures.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>canConnect()</strong>: Check if the figure can be connected to other figures.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.UngroupCommand</strong>: Clears the selection, groups and decomposes figures, and adds the decomposed figures to the selection.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Selection Management</strong>: Check if there is at least one selected figure in the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>isExecutable()</strong>: Check if there is at least one selected figure in the view.</p></li>
</ul>
</details>
<li><p><strong>Figure Grouping and Decomposition</strong>: Clears the selection, groups the selected figures, decomposes the group, and adds the decomposed figures to the selection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>execute()</strong>: Clears the selection, groups the selected figures, decomposes the group, and adds the decomposed figures to the selection.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Text Manipulation</strong>: Manipulating text figures</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.figures.NumberTextFigure</strong>: Represents a figure that displays a number as text.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Value Management</strong>: Manage the value of the figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getValue()</strong>: Return the integer value of the text in the figure, or 0 if the text cannot be parsed as an integer.</p></li>
<li><p><strong>setValue(int)</strong>: Set the value of the figure to the specified integer.</p></li>
</ul>
</details>
<li><p><strong>Overlay Calculation</strong>: Calculate the maximum number of columns needed to overlay the text.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>overlayColumns()</strong>: Return the maximum number of columns needed to overlay the text, which is either 4 or the length of the text.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.ConnectedTextTool</strong>: Activate or deactivate the ConnectedTextTool and connect text holder figure to a pressed figure if not already connected.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Activation</strong>: Set the fConnected variable to false to deactivate the tool.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>activate()</strong>: Set the `fConnected` variable to `false` to deactivate the tool.</p></li>
</ul>
</details>
<li><p><strong>Connection</strong>: Connect the text holder figure to a pressed figure if it is not already connected.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseDown(java.awt.event.MouseEvent,int,int)</strong>: Connects the text holder figure to a pressed figure if it is not already connected.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.TextTool</strong>: Activate and deactivate the TextTool and handle mouse events for editing and creating text figures.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Activation</strong>: Clear the selection and activate the TextTool.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>activate()</strong>: Clears the selection and activates the TextTool.</p></li>
</ul>
</details>
<li><p><strong>Text Editing</strong>: Begin editing the text of the figure if it is a text holder, otherwise, create a new figure and begin editing its text.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseDown(java.awt.event.MouseEvent,int,int)</strong>: Begin editing the text of the figure if it is a text holder, otherwise, create a new figure and begin editing its text.</p></li>
</ul>
</details>
<li><p><strong>Deactivation</strong>: Deactivate the text tool and end the editing process.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>deactivate()</strong>: Deactivates the text tool and ends the editing process.</p></li>
</ul>
</details>
<li><p><strong>Mouse Dragging</strong>: Drag the mouse with the given MouseEvent and coordinates.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseDrag(java.awt.event.MouseEvent,int,int)</strong>: Drag the mouse with the given MouseEvent and coordinates.</p></li>
</ul>
</details>
<li><p><strong>Mouse Up Handling</strong>: Handle the event when the mouse button is released at the specified coordinates.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseUp(java.awt.event.MouseEvent,int,int)</strong>: Handle the event when the mouse button is released at the specified coordinates.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.TextFigure</strong>: Represents a text figure that can be displayed and manipulated in a drawing.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Figure Change</strong>: Update the location of the text figure when a figure change event occurs.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureChanged(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the location of the text figure when a figure change event occurs.</p></li>
</ul>
</details>
<li><p><strong>Read-only</strong>: Manage the read-only state of the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>readOnly()</strong>: Return whether the text figure is read-only or not.</p></li>
<li><p><strong>setReadOnly(boolean)</strong>: Set the read-only state of the text figure.</p></li>
</ul>
</details>
<li><p><strong>Text Manipulation</strong>: Get and set the text of the TextFigure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getText()</strong>: Return the text of the TextFigure.</p></li>
<li><p><strong>setText(java.lang.String)</strong>: Set the text of the TextFigure to the specified new text.</p></li>
</ul>
</details>
<li><p><strong>Figure Connection</strong>: Connect and disconnect the text figure to/from other figures.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connect(CH.ifa.draw.framework.Figure)</strong>: Connects the text figure to a given figure and updates its location.</p></li>
<li><p><strong>disconnect()</strong>: Disconnects the observed figure and sets the observed figure and locator to null.</p></li>
</ul>
</details>
<li><p><strong>Font Manipulation</strong>: Manage the font used by the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setFont(java.awt.Font)</strong>: Set the font of the text figure to the specified font.</p></li>
<li><p><strong>setCurrentFontStyle(int)</strong>: Set the current font style for the TextFigure class.</p></li>
<li><p><strong>setCurrentFontName(java.lang.String)</strong>: Set the current font name to the specified name.</p></li>
<li><p><strong>setCurrentFontSize(int)</strong>: Set the current font size to the specified size.</p></li>
<li><p><strong>createCurrentFont()</strong>: Create and return a new `java.awt.Font` object using the current font name, style, and size.</p></li>
</ul>
</details>
<li><p><strong>Figure Removal</strong>: Remove a figure from the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureRequestRemove(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure specified in the FigureChangeEvent from the TextFigure.</p></li>
<li><p><strong>figureRemoved(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure from the listener if it exists.</p></li>
</ul>
</details>
<li><p><strong>Figure Display</strong>: Manage the display of the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>displayBox()</strong>: Return the bounding box of the text figure.</p></li>
<li><p><strong>overlayColumns()</strong>: Calculate the number of columns needed to overlay the text in the figure.</p></li>
<li><p><strong>handles()</strong>: Create and return a vector of handles for the TextFigure object.</p></li>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Set the origin of the text figure to the specified point.</p></li>
<li><p><strong>drawBackground(java.awt.Graphics)</strong>: Draws the background of the text figure using the given graphics object.</p></li>
<li><p><strong>drawFrame(java.awt.Graphics)</strong>: Draws the text figure's frame using the specified graphics context.</p></li>
<li><p><strong>textDisplayBox()</strong>: Return the bounding rectangle that encloses the text displayed by this TextFigure.</p></li>
</ul>
</details>
<li><p><strong>Figure Update</strong>: Update the figure based on a change event.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureRequestUpdate(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
<li><p><strong>figureInvalidated(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Invalidate the figure when a change event occurs.</p></li>
</ul>
</details>
<li><p><strong>Resource Management</strong>: Release resources held by the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>release()</strong>: Release any resources held by the TextFigure and remove it as an observer of any observed figures.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Read and write the state of the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the state of the TextFigure object to the StorableOutput stream.</p></li>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the state of a TextFigure object from a StorableInput object, including its origin, text, font, read-only status, observed figure, and locator.</p></li>
</ul>
</details>
<li><p><strong>Attribute Manipulation</strong>: Manage the attributes of the text figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setAttribute(java.lang.String,java.lang.Object)</strong>: Set the specified attribute of the TextFigure, such as font size, style, or name.</p></li>
<li><p><strong>getAttribute(java.lang.String)</strong>: Return the value of the specified attribute for the TextFigure.</p></li>
</ul>
</details>
<li><p><strong>Typing Acceptance</strong>: Check if the text figure can accept typing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>acceptsTyping()</strong>: Check if the text figure is not read-only and can accept typing.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Decoration</strong>: Adding decorations to figures</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.figures.BorderTool</strong>: Represents a tool for adding a border decoration to a figure in a drawing.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Figure Replacement</strong>: Replace the given figure in the drawing with a new figure that has a border decoration.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>action(CH.ifa.draw.framework.Figure)</strong>: Replace the given figure in the drawing with a new figure that has a border decoration.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.BorderDecorator</strong>: Calculate and display the display box of the BorderDecorator figure with specified border dimensions, update the invalidated rectangle of the figure, adjust the connection insets, and draw a border around the figure with white and gray lines.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Calculate and display display box</strong>: Calculate and return the display box of the BorderDecorator figure by growing the component's display box by the specified border dimensions.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>displayBox()</strong>: Calculate and return the display box of the BorderDecorator figure by growing the component's display box by the specified border dimensions.</p></li>
</ul>
</details>
<li><p><strong>Update invalidated rectangle</strong>: Update the invalidated rectangle of the figure with the border dimensions and notify the superclass about the figure change event.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureInvalidated(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the invalidated rectangle of the figure with the border dimensions and notify the superclass about the figure change event.</p></li>
</ul>
</details>
<li><p><strong>Adjust connection insets</strong>: Adjusts the connection insets of the figure by subtracting 3 from the top, bottom, left, and right insets.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectionInsets()</strong>: Adjusts the connection insets of the figure by subtracting 3 from the top, bottom, left, and right insets.</p></li>
</ul>
</details>
<li><p><strong>Draw border</strong>: Draws a border around the figure with white and gray lines.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws a border around the figure with white and gray lines.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>interface <strong>CH.ifa.draw.figures.LineDecoration</strong>: Represents a line decoration for a figure.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Drawing</strong>: Draws the line decoration on the given graphics object with the specified coordinates.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics,int,int,int,int)</strong>: Draws the line decoration on the given graphics object with the specified coordinates.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Management</strong>: Managing figures in a drawing</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.figures.GroupCommand</strong>: Execute group command and check if it is executable.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Execute group command</strong>: Create a new group figure with the selected figures and add it to the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>execute()</strong>: Execute the group command by creating a new group figure with the selected figures and adding it to the drawing.</p></li>
</ul>
</details>
<li><p><strong>Check if command is executable</strong>: Check if there is at least one selected figure in the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>isExecutable()</strong>: Check if there is at least one selected figure in the view.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.figures.UngroupCommand</strong>: Clears the selection, groups and decomposes figures, and adds the decomposed figures to the selection.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Selection Management</strong>: Check if there is at least one selected figure in the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>isExecutable()</strong>: Check if there is at least one selected figure in the view.</p></li>
</ul>
</details>
<li><p><strong>Figure Grouping and Decomposition</strong>: Clears the selection, groups the selected figures, decomposes the group, and adds the decomposed figures to the selection.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>execute()</strong>: Clears the selection, groups the selected figures, decomposes the group, and adds the decomposed figures to the selection.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>CH.ifa.draw.framework</strong>: Provides a framework for creating and manipulating drawings in a graphical user interface.</p></li>
<details><summary>Subgoals:</summary>
<ul>
<li><p><strong>Drawing Management</strong>: Manage the creation, modification, and deletion of drawings.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>interface <strong>CH.ifa.draw.framework.DrawingEditor</strong>: Represents a drawing editor.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Status Management</strong>: Manage the status of the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>showStatus(java.lang.String)</strong>: Show the status of the drawing editor with the given string.</p></li>
</ul>
</details>
<li><p><strong>Drawing Management</strong>: Manage the drawing associated with the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawing()</strong>: Return the drawing associated with this drawing editor.</p></li>
</ul>
</details>
<li><p><strong>Tool Management</strong>: Manage the tools used in the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>toolDone()</strong>: Finish using the current tool and return to the default state.</p></li>
<li><p><strong>tool()</strong>: Return the current tool being used in the drawing editor.</p></li>
</ul>
</details>
<li><p><strong>View Management</strong>: Manage the view of the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>view()</strong>: Return the view of the drawing editor.</p></li>
</ul>
</details>
<li><p><strong>Selection Management</strong>: Manage the selection of views in the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>selectionChanged(CH.ifa.draw.framework.DrawingView)</strong>: Set the selected view in the drawing editor to the specified view.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>interface <strong>CH.ifa.draw.framework.Drawing</strong>: Represents a drawing in a graphical user interface.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Figure Management</strong>: Manage the figures in the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>findFigure(int,int)</strong>: Find and return the figure at the specified coordinates.</p></li>
<li><p><strong>findFigure(java.awt.Rectangle,CH.ifa.draw.framework.Figure)</strong>: Find a figure within the given rectangle, excluding the specified figure.</p></li>
<li><p><strong>findFigure(java.awt.Rectangle)</strong>: Find a figure within the given rectangle.</p></li>
<li><p><strong>bringToFront(CH.ifa.draw.framework.Figure)</strong>: Bring the specified figure to the front of the drawing.</p></li>
<li><p><strong>addAll(java.util.Vector)</strong>: Add all the figures from the given vector to the drawing.</p></li>
<li><p><strong>figureRequestRemove(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure specified in the FigureChangeEvent from the drawing.</p></li>
<li><p><strong>figures()</strong>: Return an enumeration of all the figures in the drawing.</p></li>
<li><p><strong>add(CH.ifa.draw.framework.Figure)</strong>: Add a figure to the drawing.</p></li>
<li><p><strong>sendToBack(CH.ifa.draw.framework.Figure)</strong>: Move the specified figure to the back of the drawing.</p></li>
<li><p><strong>findFigureInside(int,int)</strong>: Find and return the figure located at the specified coordinates inside the drawing.</p></li>
<li><p><strong>orphan(CH.ifa.draw.framework.Figure)</strong>: Remove the specified figure from the drawing and return it.</p></li>
<li><p><strong>replace(CH.ifa.draw.framework.Figure,CH.ifa.draw.framework.Figure)</strong>: Replace a figure in the drawing with a replacement figure.</p></li>
<li><p><strong>findFigureWithout(int,int,CH.ifa.draw.framework.Figure)</strong>: Find a figure at the specified coordinates without including the specified figure.</p></li>
<li><p><strong>remove(CH.ifa.draw.framework.Figure)</strong>: Remove the specified figure from the drawing.</p></li>
<li><p><strong>findFigureInsideWithout(int,int,CH.ifa.draw.framework.Figure)</strong>: Find a figure inside the drawing at the specified coordinates, excluding the specified figure.</p></li>
<li><p><strong>removeAll(java.util.Vector)</strong>: Remove all the figures from the drawing.</p></li>
<li><p><strong>figuresReverse()</strong>: Reverse the order of the figures in the drawing and return an enumeration of the reversed figures.</p></li>
<li><p><strong>orphanAll(java.util.Vector)</strong>: Orphans all the figures in the drawing by removing them from the given vector.</p></li>
</ul>
</details>
<li><p><strong>Drawing Change Listeners</strong>: Manage the drawing change listeners.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawingChangeListeners()</strong>: Return an enumeration of the drawing change listeners registered with this drawing.</p></li>
<li><p><strong>addDrawingChangeListener(CH.ifa.draw.framework.DrawingChangeListener)</strong>: Add a drawing change listener to the drawing.</p></li>
<li><p><strong>removeDrawingChangeListener(CH.ifa.draw.framework.DrawingChangeListener)</strong>: Remove the specified DrawingChangeListener from the list of listeners for this Drawing.</p></li>
</ul>
</details>
<li><p><strong>Drawing Lock</strong>: Lock and unlock the drawing to prevent or allow modifications.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>lock()</strong>: Locks the drawing to prevent any modifications.</p></li>
<li><p><strong>unlock()</strong>: Unlock the drawing to allow modifications.</p></li>
</ul>
</details>
<li><p><strong>Figure Update</strong>: Update and invalidate figures in the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureInvalidated(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Invalidate the figure in the drawing when a FigureChangeEvent occurs.</p></li>
<li><p><strong>figureRequestUpdate(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
</ul>
</details>
<li><p><strong>Resource Management</strong>: Manage the resources held by the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>release()</strong>: Release any resources held by this drawing.</p></li>
</ul>
</details>
<li><p><strong>Drawing Representation</strong>: Draw the graphical representation of the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws the graphical representation of the object using the specified graphics context.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Management</strong>: Manage the creation, modification, and deletion of figures within a drawing.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>interface <strong>CH.ifa.draw.framework.Drawing</strong>: Represents a drawing in a graphical user interface.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Figure Management</strong>: Manage the figures in the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>findFigure(int,int)</strong>: Find and return the figure at the specified coordinates.</p></li>
<li><p><strong>findFigure(java.awt.Rectangle,CH.ifa.draw.framework.Figure)</strong>: Find a figure within the given rectangle, excluding the specified figure.</p></li>
<li><p><strong>findFigure(java.awt.Rectangle)</strong>: Find a figure within the given rectangle.</p></li>
<li><p><strong>bringToFront(CH.ifa.draw.framework.Figure)</strong>: Bring the specified figure to the front of the drawing.</p></li>
<li><p><strong>addAll(java.util.Vector)</strong>: Add all the figures from the given vector to the drawing.</p></li>
<li><p><strong>figureRequestRemove(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure specified in the FigureChangeEvent from the drawing.</p></li>
<li><p><strong>figures()</strong>: Return an enumeration of all the figures in the drawing.</p></li>
<li><p><strong>add(CH.ifa.draw.framework.Figure)</strong>: Add a figure to the drawing.</p></li>
<li><p><strong>sendToBack(CH.ifa.draw.framework.Figure)</strong>: Move the specified figure to the back of the drawing.</p></li>
<li><p><strong>findFigureInside(int,int)</strong>: Find and return the figure located at the specified coordinates inside the drawing.</p></li>
<li><p><strong>orphan(CH.ifa.draw.framework.Figure)</strong>: Remove the specified figure from the drawing and return it.</p></li>
<li><p><strong>replace(CH.ifa.draw.framework.Figure,CH.ifa.draw.framework.Figure)</strong>: Replace a figure in the drawing with a replacement figure.</p></li>
<li><p><strong>findFigureWithout(int,int,CH.ifa.draw.framework.Figure)</strong>: Find a figure at the specified coordinates without including the specified figure.</p></li>
<li><p><strong>remove(CH.ifa.draw.framework.Figure)</strong>: Remove the specified figure from the drawing.</p></li>
<li><p><strong>findFigureInsideWithout(int,int,CH.ifa.draw.framework.Figure)</strong>: Find a figure inside the drawing at the specified coordinates, excluding the specified figure.</p></li>
<li><p><strong>removeAll(java.util.Vector)</strong>: Remove all the figures from the drawing.</p></li>
<li><p><strong>figuresReverse()</strong>: Reverse the order of the figures in the drawing and return an enumeration of the reversed figures.</p></li>
<li><p><strong>orphanAll(java.util.Vector)</strong>: Orphans all the figures in the drawing by removing them from the given vector.</p></li>
</ul>
</details>
<li><p><strong>Drawing Change Listeners</strong>: Manage the drawing change listeners.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawingChangeListeners()</strong>: Return an enumeration of the drawing change listeners registered with this drawing.</p></li>
<li><p><strong>addDrawingChangeListener(CH.ifa.draw.framework.DrawingChangeListener)</strong>: Add a drawing change listener to the drawing.</p></li>
<li><p><strong>removeDrawingChangeListener(CH.ifa.draw.framework.DrawingChangeListener)</strong>: Remove the specified DrawingChangeListener from the list of listeners for this Drawing.</p></li>
</ul>
</details>
<li><p><strong>Drawing Lock</strong>: Lock and unlock the drawing to prevent or allow modifications.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>lock()</strong>: Locks the drawing to prevent any modifications.</p></li>
<li><p><strong>unlock()</strong>: Unlock the drawing to allow modifications.</p></li>
</ul>
</details>
<li><p><strong>Figure Update</strong>: Update and invalidate figures in the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureInvalidated(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Invalidate the figure in the drawing when a FigureChangeEvent occurs.</p></li>
<li><p><strong>figureRequestUpdate(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
</ul>
</details>
<li><p><strong>Resource Management</strong>: Manage the resources held by the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>release()</strong>: Release any resources held by this drawing.</p></li>
</ul>
</details>
<li><p><strong>Drawing Representation</strong>: Draw the graphical representation of the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws the graphical representation of the object using the specified graphics context.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>interface <strong>CH.ifa.draw.framework.Figure</strong>: Define the behavior of a figure in a drawing framework.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Cloning</strong>: Clone the figure object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>clone()</strong>: Clone the Figure object and return a new instance of it.</p></li>
</ul>
</details>
<li><p><strong>Displaying</strong>: Display the figure within a specified rectangle or box.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>displayBox(java.awt.Rectangle)</strong>: Display the figure within the specified rectangle.</p></li>
<li><p><strong>displayBox()</strong>: Return the bounding box of the figure.</p></li>
<li><p><strong>displayBox(java.awt.Point,java.awt.Point)</strong>: Display the box defined by the given origin and corner points.</p></li>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Set the display box of the figure using the given origin and corner points.</p></li>
</ul>
</details>
<li><p><strong>Managing Figures</strong>: Retrieve, add, and remove figures from the interface.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figures()</strong>: Return an enumeration of all the figures in the interface.</p></li>
<li><p><strong>findFigureInside(int,int)</strong>: Find and return the figure located at the specified coordinates (x, y).</p></li>
<li><p><strong>containsPoint(int,int)</strong>: Check if the figure contains the specified point.</p></li>
<li><p><strong>decompose()</strong>: Decomposes the figure into its constituent parts and returns an enumeration of them.</p></li>
<li><p><strong>isEmpty()</strong>: Check if the figure is empty.</p></li>
</ul>
</details>
<li><p><strong>Managing Attributes</strong>: Retrieve and set attributes of the figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getAttribute(java.lang.String)</strong>: Retrieve the value of the specified attribute for this Figure.</p></li>
<li><p><strong>setAttribute(java.lang.String,java.lang.Object)</strong>: Set the attribute with the given name to the specified value.</p></li>
</ul>
</details>
<li><p><strong>Managing Resources</strong>: Release any resources held by the figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>release()</strong>: Release any resources held by this figure.</p></li>
</ul>
</details>
<li><p><strong>Updating</strong>: Update the figure to reflect any changes made.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>changed()</strong>: Update the figure to reflect any changes made.</p></li>
<li><p><strong>willChange()</strong>: Notify the figure that it is about to change.</p></li>
</ul>
</details>
<li><p><strong>Moving</strong>: Move the figure by a specified amount.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>moveBy(int,int)</strong>: Move the figure by the specified amount in the x and y directions.</p></li>
</ul>
</details>
<li><p><strong>Connecting</strong>: Check if the figure can be connected to another figure and return the connector at specified coordinates.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>canConnect()</strong>: Check if the figure can be connected to another figure.</p></li>
<li><p><strong>connectorAt(int,int)</strong>: Return the connector at the specified coordinates.</p></li>
</ul>
</details>
<li><p><strong>Handling</strong>: Return handles and a listener for the figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>listener()</strong>: Return the listener for this figure.</p></li>
<li><p><strong>handles()</strong>: Return a vector of handles for this figure.</p></li>
</ul>
</details>
<li><p><strong>Managing Change Listeners</strong>: Add and remove FigureChangeListeners from the figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>addToContainer(CH.ifa.draw.framework.FigureChangeListener)</strong>: Add a FigureChangeListener to the container.</p></li>
<li><p><strong>removeFromContainer(CH.ifa.draw.framework.FigureChangeListener)</strong>: Remove the specified FigureChangeListener from the container.</p></li>
<li><p><strong>addFigureChangeListener(CH.ifa.draw.framework.FigureChangeListener)</strong>: Add a FigureChangeListener to the list of listeners for this Figure.</p></li>
<li><p><strong>removeFigureChangeListener(CH.ifa.draw.framework.FigureChangeListener)</strong>: (no description)</p></li>
</ul>
</details>
<li><p><strong>Miscellaneous</strong>: Invalidate the figure, check if a given figure is included within this figure, return the bounding box, center point, size, and connection insets of the figure, and return a locator for the connected text of a given figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invalidate()</strong>: Invalidate the figure to indicate that it needs to be redrawn.</p></li>
<li><p><strong>includes(CH.ifa.draw.framework.Figure)</strong>: Check if the given figure is included within this figure.</p></li>
<li><p><strong>connectionInsets()</strong>: Return the connection insets of the figure.</p></li>
<li><p><strong>connectedTextLocator(CH.ifa.draw.framework.Figure)</strong>: Return a locator for the connected text of the given figure.</p></li>
<li><p><strong>size()</strong>: Return the size of the figure.</p></li>
<li><p><strong>center()</strong>: Return the center point of the figure.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Tool Management</strong>: Manage the activation and deactivation of tools for interacting with the drawing.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>interface <strong>CH.ifa.draw.framework.DrawingEditor</strong>: Represents a drawing editor.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Status Management</strong>: Manage the status of the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>showStatus(java.lang.String)</strong>: Show the status of the drawing editor with the given string.</p></li>
</ul>
</details>
<li><p><strong>Drawing Management</strong>: Manage the drawing associated with the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawing()</strong>: Return the drawing associated with this drawing editor.</p></li>
</ul>
</details>
<li><p><strong>Tool Management</strong>: Manage the tools used in the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>toolDone()</strong>: Finish using the current tool and return to the default state.</p></li>
<li><p><strong>tool()</strong>: Return the current tool being used in the drawing editor.</p></li>
</ul>
</details>
<li><p><strong>View Management</strong>: Manage the view of the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>view()</strong>: Return the view of the drawing editor.</p></li>
</ul>
</details>
<li><p><strong>Selection Management</strong>: Manage the selection of views in the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>selectionChanged(CH.ifa.draw.framework.DrawingView)</strong>: Set the selected view in the drawing editor to the specified view.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>interface <strong>CH.ifa.draw.framework.Tool</strong>: This interface represents a tool in a drawing framework.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Mouse Events</strong>: Handle mouse events such as mouse up, mouse drag, mouse down, mouse move.</p></li>
<details><summary>Methods involved:</summary>
<ul>
</ul>
</details>
<li><p><strong>Key Events</strong>: Handle key events when a key is pressed down.</p></li>
<details><summary>Methods involved:</summary>
<ul>
</ul>
</details>
<li><p><strong>Activation/Deactivation</strong>: Activate or deactivate the tool.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>activate()</strong>: Activate the tool.</p></li>
<li><p><strong>deactivate()</strong>: Deactivate the tool.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>View Management</strong>: Manage the display and interaction with the drawing view.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>interface <strong>CH.ifa.draw.framework.DrawingEditor</strong>: Represents a drawing editor.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Status Management</strong>: Manage the status of the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>showStatus(java.lang.String)</strong>: Show the status of the drawing editor with the given string.</p></li>
</ul>
</details>
<li><p><strong>Drawing Management</strong>: Manage the drawing associated with the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawing()</strong>: Return the drawing associated with this drawing editor.</p></li>
</ul>
</details>
<li><p><strong>Tool Management</strong>: Manage the tools used in the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>toolDone()</strong>: Finish using the current tool and return to the default state.</p></li>
<li><p><strong>tool()</strong>: Return the current tool being used in the drawing editor.</p></li>
</ul>
</details>
<li><p><strong>View Management</strong>: Manage the view of the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>view()</strong>: Return the view of the drawing editor.</p></li>
</ul>
</details>
<li><p><strong>Selection Management</strong>: Manage the selection of views in the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>selectionChanged(CH.ifa.draw.framework.DrawingView)</strong>: Set the selected view in the drawing editor to the specified view.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>interface <strong>CH.ifa.draw.framework.DrawingView</strong>: Represents a view of a drawing with various methods for manipulating and interacting with the drawing.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Selection</strong>: Methods related to selecting figures in the drawing view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>selectionElements()</strong>: Return an enumeration of the selected figures in the drawing view.</p></li>
<li><p><strong>getFigureSelection()</strong>: Return the selected figures in the drawing view.</p></li>
<li><p><strong>toggleSelection(CH.ifa.draw.framework.Figure)</strong>: Toggle the selection state of the given figure in the drawing view.</p></li>
<li><p><strong>removeFromSelection(CH.ifa.draw.framework.Figure)</strong>: Remove the specified figure from the selection in the drawing view.</p></li>
<li><p><strong>selection()</strong>: Return the selected objects in the drawing view as a vector.</p></li>
<li><p><strong>selectionZOrdered()</strong>: Return a vector containing the selected objects in the drawing view, ordered by their Z-order.</p></li>
<li><p><strong>selectionCount()</strong>: Return the number of selected objects in the drawing view.</p></li>
<li><p><strong>clearSelection()</strong>: Clears the current selection of objects in the drawing view.</p></li>
<li><p><strong>addToSelection(CH.ifa.draw.framework.Figure)</strong>: Add the specified figure to the current selection.</p></li>
<li><p><strong>addToSelectionAll(java.util.Vector)</strong>: Add all the figures in the given vector to the current selection.</p></li>
</ul>
</details>
<li><p><strong>Editor</strong>: Methods related to setting and retrieving the editor for the drawing view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setEditor(CH.ifa.draw.framework.DrawingEditor)</strong>: Set the editor for this drawing view.</p></li>
<li><p><strong>editor()</strong>: Return the drawing editor associated with this drawing view.</p></li>
</ul>
</details>
<li><p><strong>Drawing</strong>: Methods related to setting and retrieving the drawing associated with the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setDrawing(CH.ifa.draw.framework.Drawing)</strong>: Set the drawing for this drawing view.</p></li>
<li><p><strong>drawing()</strong>: Return the drawing associated with this view.</p></li>
</ul>
</details>
<li><p><strong>Graphics</strong>: Methods related to drawing and painting on the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawDrawing(java.awt.Graphics)</strong>: Draws the drawing on the specified graphics context.</p></li>
<li><p><strong>getGraphics()</strong>: Return the graphics object used for drawing on this view.</p></li>
<li><p><strong>drawBackground(java.awt.Graphics)</strong>: Draws the background of the drawing view using the specified graphics context.</p></li>
<li><p><strong>paint(java.awt.Graphics)</strong>: Paints the graphics of the drawing view.</p></li>
<li><p><strong>drawHandles(java.awt.Graphics)</strong>: Draws the handles of the drawing view using the specified graphics context.</p></li>
<li><p><strong>drawAll(java.awt.Graphics)</strong>: Draws all the elements in the drawing view using the specified graphics context.</p></li>
<li><p><strong>createImage(int,int)</strong>: Create an image with the specified width and height.</p></li>
</ul>
</details>
<li><p><strong>Size</strong>: Methods related to getting the size of the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getMinimumSize()</strong>: Return the minimum size of the drawing view.</p></li>
<li><p><strong>getSize()</strong>: Return the size of the drawing view.</p></li>
<li><p><strong>getPreferredSize()</strong>: Return the preferred size of the drawing view.</p></li>
</ul>
</details>
<li><p><strong>Background</strong>: Methods related to setting and retrieving the background color of the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getBackground()</strong>: Return the background color of the drawing view.</p></li>
<li><p><strong>setBackground(java.awt.Color)</strong>: Set the background color of the drawing view to the specified color.</p></li>
</ul>
</details>
<li><p><strong>Interaction</strong>: Methods related to freezing and unfreezing the view for user interaction.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>unfreezeView()</strong>: Unfreezes the view to allow for user interaction.</p></li>
<li><p><strong>freezeView()</strong>: Freezes the current view of the drawing.</p></li>
</ul>
</details>
<li><p><strong>Constrainer</strong>: Methods related to setting and retrieving the point constrainer for the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getConstrainer()</strong>: Return the constrainer object used by this drawing view.</p></li>
<li><p><strong>setConstrainer(CH.ifa.draw.framework.PointConstrainer)</strong>: Set the point constrainer for this drawing view.</p></li>
</ul>
</details>
<li><p><strong>Handle</strong>: Methods related to finding and manipulating handles on the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>findHandle(int,int)</strong>: Find and return the handle at the specified coordinates.</p></li>
</ul>
</details>
<li><p><strong>Update</strong>: Methods related to setting the update strategy for displaying the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setDisplayUpdate(CH.ifa.draw.framework.Painter)</strong>: Set the update strategy for displaying the drawing view.</p></li>
</ul>
</details>
<li><p><strong>Repair</strong>: Methods related to checking and repairing damage to the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>checkDamage()</strong>: Check the damage caused to the drawing view.</p></li>
<li><p><strong>repairDamage()</strong>: Repair any damage to the drawing view.</p></li>
</ul>
</details>
<li><p><strong>Figure</strong>: Methods related to adding, removing, and retrieving figures in the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>add(CH.ifa.draw.framework.Figure)</strong>: Add a figure to the drawing view.</p></li>
<li><p><strong>remove(CH.ifa.draw.framework.Figure)</strong>: Remove the specified figure from the drawing view.</p></li>
<li><p><strong>getFigureSelection()</strong>: Return the selected figures in the drawing view.</p></li>
<li><p><strong>addAll(java.util.Vector)</strong>: Add all the figures from the given vector to the drawing view.</p></li>
</ul>
</details>
<li><p><strong>Tool</strong>: Methods related to retrieving the tool used by the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>tool()</strong>: Return the tool used by this drawing view.</p></li>
</ul>
</details>
<li><p><strong>Last Click</strong>: Methods related to retrieving the last clicked point in the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>lastClick()</strong>: Return the last clicked point in the drawing view.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Selection Management</strong>: Manage the selection of figures within the drawing.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>interface <strong>CH.ifa.draw.framework.DrawingEditor</strong>: Represents a drawing editor.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Status Management</strong>: Manage the status of the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>showStatus(java.lang.String)</strong>: Show the status of the drawing editor with the given string.</p></li>
</ul>
</details>
<li><p><strong>Drawing Management</strong>: Manage the drawing associated with the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawing()</strong>: Return the drawing associated with this drawing editor.</p></li>
</ul>
</details>
<li><p><strong>Tool Management</strong>: Manage the tools used in the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>toolDone()</strong>: Finish using the current tool and return to the default state.</p></li>
<li><p><strong>tool()</strong>: Return the current tool being used in the drawing editor.</p></li>
</ul>
</details>
<li><p><strong>View Management</strong>: Manage the view of the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>view()</strong>: Return the view of the drawing editor.</p></li>
</ul>
</details>
<li><p><strong>Selection Management</strong>: Manage the selection of views in the drawing editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>selectionChanged(CH.ifa.draw.framework.DrawingView)</strong>: Set the selected view in the drawing editor to the specified view.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>interface <strong>CH.ifa.draw.framework.DrawingView</strong>: Represents a view of a drawing with various methods for manipulating and interacting with the drawing.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Selection</strong>: Methods related to selecting figures in the drawing view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>selectionElements()</strong>: Return an enumeration of the selected figures in the drawing view.</p></li>
<li><p><strong>getFigureSelection()</strong>: Return the selected figures in the drawing view.</p></li>
<li><p><strong>toggleSelection(CH.ifa.draw.framework.Figure)</strong>: Toggle the selection state of the given figure in the drawing view.</p></li>
<li><p><strong>removeFromSelection(CH.ifa.draw.framework.Figure)</strong>: Remove the specified figure from the selection in the drawing view.</p></li>
<li><p><strong>selection()</strong>: Return the selected objects in the drawing view as a vector.</p></li>
<li><p><strong>selectionZOrdered()</strong>: Return a vector containing the selected objects in the drawing view, ordered by their Z-order.</p></li>
<li><p><strong>selectionCount()</strong>: Return the number of selected objects in the drawing view.</p></li>
<li><p><strong>clearSelection()</strong>: Clears the current selection of objects in the drawing view.</p></li>
<li><p><strong>addToSelection(CH.ifa.draw.framework.Figure)</strong>: Add the specified figure to the current selection.</p></li>
<li><p><strong>addToSelectionAll(java.util.Vector)</strong>: Add all the figures in the given vector to the current selection.</p></li>
</ul>
</details>
<li><p><strong>Editor</strong>: Methods related to setting and retrieving the editor for the drawing view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setEditor(CH.ifa.draw.framework.DrawingEditor)</strong>: Set the editor for this drawing view.</p></li>
<li><p><strong>editor()</strong>: Return the drawing editor associated with this drawing view.</p></li>
</ul>
</details>
<li><p><strong>Drawing</strong>: Methods related to setting and retrieving the drawing associated with the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setDrawing(CH.ifa.draw.framework.Drawing)</strong>: Set the drawing for this drawing view.</p></li>
<li><p><strong>drawing()</strong>: Return the drawing associated with this view.</p></li>
</ul>
</details>
<li><p><strong>Graphics</strong>: Methods related to drawing and painting on the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawDrawing(java.awt.Graphics)</strong>: Draws the drawing on the specified graphics context.</p></li>
<li><p><strong>getGraphics()</strong>: Return the graphics object used for drawing on this view.</p></li>
<li><p><strong>drawBackground(java.awt.Graphics)</strong>: Draws the background of the drawing view using the specified graphics context.</p></li>
<li><p><strong>paint(java.awt.Graphics)</strong>: Paints the graphics of the drawing view.</p></li>
<li><p><strong>drawHandles(java.awt.Graphics)</strong>: Draws the handles of the drawing view using the specified graphics context.</p></li>
<li><p><strong>drawAll(java.awt.Graphics)</strong>: Draws all the elements in the drawing view using the specified graphics context.</p></li>
<li><p><strong>createImage(int,int)</strong>: Create an image with the specified width and height.</p></li>
</ul>
</details>
<li><p><strong>Size</strong>: Methods related to getting the size of the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getMinimumSize()</strong>: Return the minimum size of the drawing view.</p></li>
<li><p><strong>getSize()</strong>: Return the size of the drawing view.</p></li>
<li><p><strong>getPreferredSize()</strong>: Return the preferred size of the drawing view.</p></li>
</ul>
</details>
<li><p><strong>Background</strong>: Methods related to setting and retrieving the background color of the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getBackground()</strong>: Return the background color of the drawing view.</p></li>
<li><p><strong>setBackground(java.awt.Color)</strong>: Set the background color of the drawing view to the specified color.</p></li>
</ul>
</details>
<li><p><strong>Interaction</strong>: Methods related to freezing and unfreezing the view for user interaction.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>unfreezeView()</strong>: Unfreezes the view to allow for user interaction.</p></li>
<li><p><strong>freezeView()</strong>: Freezes the current view of the drawing.</p></li>
</ul>
</details>
<li><p><strong>Constrainer</strong>: Methods related to setting and retrieving the point constrainer for the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getConstrainer()</strong>: Return the constrainer object used by this drawing view.</p></li>
<li><p><strong>setConstrainer(CH.ifa.draw.framework.PointConstrainer)</strong>: Set the point constrainer for this drawing view.</p></li>
</ul>
</details>
<li><p><strong>Handle</strong>: Methods related to finding and manipulating handles on the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>findHandle(int,int)</strong>: Find and return the handle at the specified coordinates.</p></li>
</ul>
</details>
<li><p><strong>Update</strong>: Methods related to setting the update strategy for displaying the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setDisplayUpdate(CH.ifa.draw.framework.Painter)</strong>: Set the update strategy for displaying the drawing view.</p></li>
</ul>
</details>
<li><p><strong>Repair</strong>: Methods related to checking and repairing damage to the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>checkDamage()</strong>: Check the damage caused to the drawing view.</p></li>
<li><p><strong>repairDamage()</strong>: Repair any damage to the drawing view.</p></li>
</ul>
</details>
<li><p><strong>Figure</strong>: Methods related to adding, removing, and retrieving figures in the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>add(CH.ifa.draw.framework.Figure)</strong>: Add a figure to the drawing view.</p></li>
<li><p><strong>remove(CH.ifa.draw.framework.Figure)</strong>: Remove the specified figure from the drawing view.</p></li>
<li><p><strong>getFigureSelection()</strong>: Return the selected figures in the drawing view.</p></li>
<li><p><strong>addAll(java.util.Vector)</strong>: Add all the figures from the given vector to the drawing view.</p></li>
</ul>
</details>
<li><p><strong>Tool</strong>: Methods related to retrieving the tool used by the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>tool()</strong>: Return the tool used by this drawing view.</p></li>
</ul>
</details>
<li><p><strong>Last Click</strong>: Methods related to retrieving the last clicked point in the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>lastClick()</strong>: Return the last clicked point in the drawing view.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Enumeration</strong>: Enumerate the figures within a drawing.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>interface <strong>CH.ifa.draw.framework.FigureEnumeration</strong>: Enumerates figures.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Figure Enumeration</strong>: Iterates through a collection of figures.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>nextFigure()</strong>: Return the next figure in the enumeration.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Manipulation</strong>: Manipulate the position and size of figures within the drawing.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>interface <strong>CH.ifa.draw.framework.ConnectionFigure</strong>: Represents a connection figure between two figures.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Connection Management</strong>: Manage the connection between two figures.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>endPoint(int,int)</strong>: Set the end point of the connection figure to the specified coordinates.</p></li>
<li><p><strong>startPoint(int,int)</strong>: Set the starting point of the connection figure to the specified coordinates.</p></li>
</ul>
</details>
<li><p><strong>Figure Manipulation</strong>: Manipulate the points and segments of the connection figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>startPoint(int,int)</strong>: Set the starting point of the connection figure to the specified coordinates.</p></li>
<li><p><strong>endPoint(int,int)</strong>: Set the end point of the connection figure to the specified coordinates.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Update</strong>: Update the appearance and state of figures within the drawing.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>interface <strong>CH.ifa.draw.framework.Drawing</strong>: Represents a drawing in a graphical user interface.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Figure Management</strong>: Manage the figures in the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>findFigure(int,int)</strong>: Find and return the figure at the specified coordinates.</p></li>
<li><p><strong>findFigure(java.awt.Rectangle,CH.ifa.draw.framework.Figure)</strong>: Find a figure within the given rectangle, excluding the specified figure.</p></li>
<li><p><strong>findFigure(java.awt.Rectangle)</strong>: Find a figure within the given rectangle.</p></li>
<li><p><strong>bringToFront(CH.ifa.draw.framework.Figure)</strong>: Bring the specified figure to the front of the drawing.</p></li>
<li><p><strong>addAll(java.util.Vector)</strong>: Add all the figures from the given vector to the drawing.</p></li>
<li><p><strong>figureRequestRemove(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure specified in the FigureChangeEvent from the drawing.</p></li>
<li><p><strong>figures()</strong>: Return an enumeration of all the figures in the drawing.</p></li>
<li><p><strong>add(CH.ifa.draw.framework.Figure)</strong>: Add a figure to the drawing.</p></li>
<li><p><strong>sendToBack(CH.ifa.draw.framework.Figure)</strong>: Move the specified figure to the back of the drawing.</p></li>
<li><p><strong>findFigureInside(int,int)</strong>: Find and return the figure located at the specified coordinates inside the drawing.</p></li>
<li><p><strong>orphan(CH.ifa.draw.framework.Figure)</strong>: Remove the specified figure from the drawing and return it.</p></li>
<li><p><strong>replace(CH.ifa.draw.framework.Figure,CH.ifa.draw.framework.Figure)</strong>: Replace a figure in the drawing with a replacement figure.</p></li>
<li><p><strong>findFigureWithout(int,int,CH.ifa.draw.framework.Figure)</strong>: Find a figure at the specified coordinates without including the specified figure.</p></li>
<li><p><strong>remove(CH.ifa.draw.framework.Figure)</strong>: Remove the specified figure from the drawing.</p></li>
<li><p><strong>findFigureInsideWithout(int,int,CH.ifa.draw.framework.Figure)</strong>: Find a figure inside the drawing at the specified coordinates, excluding the specified figure.</p></li>
<li><p><strong>removeAll(java.util.Vector)</strong>: Remove all the figures from the drawing.</p></li>
<li><p><strong>figuresReverse()</strong>: Reverse the order of the figures in the drawing and return an enumeration of the reversed figures.</p></li>
<li><p><strong>orphanAll(java.util.Vector)</strong>: Orphans all the figures in the drawing by removing them from the given vector.</p></li>
</ul>
</details>
<li><p><strong>Drawing Change Listeners</strong>: Manage the drawing change listeners.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawingChangeListeners()</strong>: Return an enumeration of the drawing change listeners registered with this drawing.</p></li>
<li><p><strong>addDrawingChangeListener(CH.ifa.draw.framework.DrawingChangeListener)</strong>: Add a drawing change listener to the drawing.</p></li>
<li><p><strong>removeDrawingChangeListener(CH.ifa.draw.framework.DrawingChangeListener)</strong>: Remove the specified DrawingChangeListener from the list of listeners for this Drawing.</p></li>
</ul>
</details>
<li><p><strong>Drawing Lock</strong>: Lock and unlock the drawing to prevent or allow modifications.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>lock()</strong>: Locks the drawing to prevent any modifications.</p></li>
<li><p><strong>unlock()</strong>: Unlock the drawing to allow modifications.</p></li>
</ul>
</details>
<li><p><strong>Figure Update</strong>: Update and invalidate figures in the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureInvalidated(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Invalidate the figure in the drawing when a FigureChangeEvent occurs.</p></li>
<li><p><strong>figureRequestUpdate(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
</ul>
</details>
<li><p><strong>Resource Management</strong>: Manage the resources held by the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>release()</strong>: Release any resources held by this drawing.</p></li>
</ul>
</details>
<li><p><strong>Drawing Representation</strong>: Draw the graphical representation of the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws the graphical representation of the object using the specified graphics context.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>interface <strong>CH.ifa.draw.framework.Figure</strong>: Define the behavior of a figure in a drawing framework.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Cloning</strong>: Clone the figure object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>clone()</strong>: Clone the Figure object and return a new instance of it.</p></li>
</ul>
</details>
<li><p><strong>Displaying</strong>: Display the figure within a specified rectangle or box.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>displayBox(java.awt.Rectangle)</strong>: Display the figure within the specified rectangle.</p></li>
<li><p><strong>displayBox()</strong>: Return the bounding box of the figure.</p></li>
<li><p><strong>displayBox(java.awt.Point,java.awt.Point)</strong>: Display the box defined by the given origin and corner points.</p></li>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Set the display box of the figure using the given origin and corner points.</p></li>
</ul>
</details>
<li><p><strong>Managing Figures</strong>: Retrieve, add, and remove figures from the interface.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figures()</strong>: Return an enumeration of all the figures in the interface.</p></li>
<li><p><strong>findFigureInside(int,int)</strong>: Find and return the figure located at the specified coordinates (x, y).</p></li>
<li><p><strong>containsPoint(int,int)</strong>: Check if the figure contains the specified point.</p></li>
<li><p><strong>decompose()</strong>: Decomposes the figure into its constituent parts and returns an enumeration of them.</p></li>
<li><p><strong>isEmpty()</strong>: Check if the figure is empty.</p></li>
</ul>
</details>
<li><p><strong>Managing Attributes</strong>: Retrieve and set attributes of the figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getAttribute(java.lang.String)</strong>: Retrieve the value of the specified attribute for this Figure.</p></li>
<li><p><strong>setAttribute(java.lang.String,java.lang.Object)</strong>: Set the attribute with the given name to the specified value.</p></li>
</ul>
</details>
<li><p><strong>Managing Resources</strong>: Release any resources held by the figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>release()</strong>: Release any resources held by this figure.</p></li>
</ul>
</details>
<li><p><strong>Updating</strong>: Update the figure to reflect any changes made.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>changed()</strong>: Update the figure to reflect any changes made.</p></li>
<li><p><strong>willChange()</strong>: Notify the figure that it is about to change.</p></li>
</ul>
</details>
<li><p><strong>Moving</strong>: Move the figure by a specified amount.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>moveBy(int,int)</strong>: Move the figure by the specified amount in the x and y directions.</p></li>
</ul>
</details>
<li><p><strong>Connecting</strong>: Check if the figure can be connected to another figure and return the connector at specified coordinates.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>canConnect()</strong>: Check if the figure can be connected to another figure.</p></li>
<li><p><strong>connectorAt(int,int)</strong>: Return the connector at the specified coordinates.</p></li>
</ul>
</details>
<li><p><strong>Handling</strong>: Return handles and a listener for the figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>listener()</strong>: Return the listener for this figure.</p></li>
<li><p><strong>handles()</strong>: Return a vector of handles for this figure.</p></li>
</ul>
</details>
<li><p><strong>Managing Change Listeners</strong>: Add and remove FigureChangeListeners from the figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>addToContainer(CH.ifa.draw.framework.FigureChangeListener)</strong>: Add a FigureChangeListener to the container.</p></li>
<li><p><strong>removeFromContainer(CH.ifa.draw.framework.FigureChangeListener)</strong>: Remove the specified FigureChangeListener from the container.</p></li>
<li><p><strong>addFigureChangeListener(CH.ifa.draw.framework.FigureChangeListener)</strong>: Add a FigureChangeListener to the list of listeners for this Figure.</p></li>
<li><p><strong>removeFigureChangeListener(CH.ifa.draw.framework.FigureChangeListener)</strong>: (no description)</p></li>
</ul>
</details>
<li><p><strong>Miscellaneous</strong>: Invalidate the figure, check if a given figure is included within this figure, return the bounding box, center point, size, and connection insets of the figure, and return a locator for the connected text of a given figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>invalidate()</strong>: Invalidate the figure to indicate that it needs to be redrawn.</p></li>
<li><p><strong>includes(CH.ifa.draw.framework.Figure)</strong>: Check if the given figure is included within this figure.</p></li>
<li><p><strong>connectionInsets()</strong>: Return the connection insets of the figure.</p></li>
<li><p><strong>connectedTextLocator(CH.ifa.draw.framework.Figure)</strong>: Return a locator for the connected text of the given figure.</p></li>
<li><p><strong>size()</strong>: Return the size of the figure.</p></li>
<li><p><strong>center()</strong>: Return the center point of the figure.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Change Listeners</strong>: Handle and respond to changes in figures within the drawing.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>interface <strong>CH.ifa.draw.framework.Drawing</strong>: Represents a drawing in a graphical user interface.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Figure Management</strong>: Manage the figures in the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>findFigure(int,int)</strong>: Find and return the figure at the specified coordinates.</p></li>
<li><p><strong>findFigure(java.awt.Rectangle,CH.ifa.draw.framework.Figure)</strong>: Find a figure within the given rectangle, excluding the specified figure.</p></li>
<li><p><strong>findFigure(java.awt.Rectangle)</strong>: Find a figure within the given rectangle.</p></li>
<li><p><strong>bringToFront(CH.ifa.draw.framework.Figure)</strong>: Bring the specified figure to the front of the drawing.</p></li>
<li><p><strong>addAll(java.util.Vector)</strong>: Add all the figures from the given vector to the drawing.</p></li>
<li><p><strong>figureRequestRemove(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure specified in the FigureChangeEvent from the drawing.</p></li>
<li><p><strong>figures()</strong>: Return an enumeration of all the figures in the drawing.</p></li>
<li><p><strong>add(CH.ifa.draw.framework.Figure)</strong>: Add a figure to the drawing.</p></li>
<li><p><strong>sendToBack(CH.ifa.draw.framework.Figure)</strong>: Move the specified figure to the back of the drawing.</p></li>
<li><p><strong>findFigureInside(int,int)</strong>: Find and return the figure located at the specified coordinates inside the drawing.</p></li>
<li><p><strong>orphan(CH.ifa.draw.framework.Figure)</strong>: Remove the specified figure from the drawing and return it.</p></li>
<li><p><strong>replace(CH.ifa.draw.framework.Figure,CH.ifa.draw.framework.Figure)</strong>: Replace a figure in the drawing with a replacement figure.</p></li>
<li><p><strong>findFigureWithout(int,int,CH.ifa.draw.framework.Figure)</strong>: Find a figure at the specified coordinates without including the specified figure.</p></li>
<li><p><strong>remove(CH.ifa.draw.framework.Figure)</strong>: Remove the specified figure from the drawing.</p></li>
<li><p><strong>findFigureInsideWithout(int,int,CH.ifa.draw.framework.Figure)</strong>: Find a figure inside the drawing at the specified coordinates, excluding the specified figure.</p></li>
<li><p><strong>removeAll(java.util.Vector)</strong>: Remove all the figures from the drawing.</p></li>
<li><p><strong>figuresReverse()</strong>: Reverse the order of the figures in the drawing and return an enumeration of the reversed figures.</p></li>
<li><p><strong>orphanAll(java.util.Vector)</strong>: Orphans all the figures in the drawing by removing them from the given vector.</p></li>
</ul>
</details>
<li><p><strong>Drawing Change Listeners</strong>: Manage the drawing change listeners.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawingChangeListeners()</strong>: Return an enumeration of the drawing change listeners registered with this drawing.</p></li>
<li><p><strong>addDrawingChangeListener(CH.ifa.draw.framework.DrawingChangeListener)</strong>: Add a drawing change listener to the drawing.</p></li>
<li><p><strong>removeDrawingChangeListener(CH.ifa.draw.framework.DrawingChangeListener)</strong>: Remove the specified DrawingChangeListener from the list of listeners for this Drawing.</p></li>
</ul>
</details>
<li><p><strong>Drawing Lock</strong>: Lock and unlock the drawing to prevent or allow modifications.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>lock()</strong>: Locks the drawing to prevent any modifications.</p></li>
<li><p><strong>unlock()</strong>: Unlock the drawing to allow modifications.</p></li>
</ul>
</details>
<li><p><strong>Figure Update</strong>: Update and invalidate figures in the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureInvalidated(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Invalidate the figure in the drawing when a FigureChangeEvent occurs.</p></li>
<li><p><strong>figureRequestUpdate(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
</ul>
</details>
<li><p><strong>Resource Management</strong>: Manage the resources held by the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>release()</strong>: Release any resources held by this drawing.</p></li>
</ul>
</details>
<li><p><strong>Drawing Representation</strong>: Draw the graphical representation of the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws the graphical representation of the object using the specified graphics context.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>interface <strong>CH.ifa.draw.framework.FigureChangeListener</strong>: This interface defines the behavior of a FigureChangeListener.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Figure Removal</strong>: Remove a figure from the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureRemoved(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove a figure from the drawing.</p></li>
</ul>
</details>
<li><p><strong>Figure Update</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureRequestUpdate(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
<li><p><strong>figureChanged(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
</ul>
</details>
<li><p><strong>Figure Invalidation</strong>: Invalidate the figure in response to a FigureChangeEvent.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureInvalidated(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Invalidate the figure in response to a FigureChangeEvent.</p></li>
</ul>
</details>
<li><p><strong>Figure Removal Request</strong>: Remove the figure specified in the FigureChangeEvent from the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureRequestRemove(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure specified in the FigureChangeEvent from the drawing.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.framework.FigureChangeEvent</strong>: Represents a change event for a figure.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Figure Access</strong>: Provides access to the figure associated with this FigureChangeEvent.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getFigure()</strong>: Return the figure associated with this FigureChangeEvent.</p></li>
</ul>
</details>
<li><p><strong>Invalidated Rectangle Access</strong>: Provides access to the rectangle that represents the area invalidated by the figure change event.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getInvalidatedRectangle()</strong>: Return the rectangle that represents the area invalidated by the figure change event.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Drawing Change Listeners</strong>: Handle and respond to changes in the drawing.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>interface <strong>CH.ifa.draw.framework.Drawing</strong>: Represents a drawing in a graphical user interface.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Figure Management</strong>: Manage the figures in the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>findFigure(int,int)</strong>: Find and return the figure at the specified coordinates.</p></li>
<li><p><strong>findFigure(java.awt.Rectangle,CH.ifa.draw.framework.Figure)</strong>: Find a figure within the given rectangle, excluding the specified figure.</p></li>
<li><p><strong>findFigure(java.awt.Rectangle)</strong>: Find a figure within the given rectangle.</p></li>
<li><p><strong>bringToFront(CH.ifa.draw.framework.Figure)</strong>: Bring the specified figure to the front of the drawing.</p></li>
<li><p><strong>addAll(java.util.Vector)</strong>: Add all the figures from the given vector to the drawing.</p></li>
<li><p><strong>figureRequestRemove(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure specified in the FigureChangeEvent from the drawing.</p></li>
<li><p><strong>figures()</strong>: Return an enumeration of all the figures in the drawing.</p></li>
<li><p><strong>add(CH.ifa.draw.framework.Figure)</strong>: Add a figure to the drawing.</p></li>
<li><p><strong>sendToBack(CH.ifa.draw.framework.Figure)</strong>: Move the specified figure to the back of the drawing.</p></li>
<li><p><strong>findFigureInside(int,int)</strong>: Find and return the figure located at the specified coordinates inside the drawing.</p></li>
<li><p><strong>orphan(CH.ifa.draw.framework.Figure)</strong>: Remove the specified figure from the drawing and return it.</p></li>
<li><p><strong>replace(CH.ifa.draw.framework.Figure,CH.ifa.draw.framework.Figure)</strong>: Replace a figure in the drawing with a replacement figure.</p></li>
<li><p><strong>findFigureWithout(int,int,CH.ifa.draw.framework.Figure)</strong>: Find a figure at the specified coordinates without including the specified figure.</p></li>
<li><p><strong>remove(CH.ifa.draw.framework.Figure)</strong>: Remove the specified figure from the drawing.</p></li>
<li><p><strong>findFigureInsideWithout(int,int,CH.ifa.draw.framework.Figure)</strong>: Find a figure inside the drawing at the specified coordinates, excluding the specified figure.</p></li>
<li><p><strong>removeAll(java.util.Vector)</strong>: Remove all the figures from the drawing.</p></li>
<li><p><strong>figuresReverse()</strong>: Reverse the order of the figures in the drawing and return an enumeration of the reversed figures.</p></li>
<li><p><strong>orphanAll(java.util.Vector)</strong>: Orphans all the figures in the drawing by removing them from the given vector.</p></li>
</ul>
</details>
<li><p><strong>Drawing Change Listeners</strong>: Manage the drawing change listeners.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawingChangeListeners()</strong>: Return an enumeration of the drawing change listeners registered with this drawing.</p></li>
<li><p><strong>addDrawingChangeListener(CH.ifa.draw.framework.DrawingChangeListener)</strong>: Add a drawing change listener to the drawing.</p></li>
<li><p><strong>removeDrawingChangeListener(CH.ifa.draw.framework.DrawingChangeListener)</strong>: Remove the specified DrawingChangeListener from the list of listeners for this Drawing.</p></li>
</ul>
</details>
<li><p><strong>Drawing Lock</strong>: Lock and unlock the drawing to prevent or allow modifications.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>lock()</strong>: Locks the drawing to prevent any modifications.</p></li>
<li><p><strong>unlock()</strong>: Unlock the drawing to allow modifications.</p></li>
</ul>
</details>
<li><p><strong>Figure Update</strong>: Update and invalidate figures in the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureInvalidated(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Invalidate the figure in the drawing when a FigureChangeEvent occurs.</p></li>
<li><p><strong>figureRequestUpdate(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the figure based on the given FigureChangeEvent.</p></li>
</ul>
</details>
<li><p><strong>Resource Management</strong>: Manage the resources held by the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>release()</strong>: Release any resources held by this drawing.</p></li>
</ul>
</details>
<li><p><strong>Drawing Representation</strong>: Draw the graphical representation of the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws the graphical representation of the object using the specified graphics context.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>interface <strong>CH.ifa.draw.framework.DrawingChangeListener</strong>: Update and invalidate the drawing based on drawing change events.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Update Drawing</strong>: Update the drawing based on the given drawing change event.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawingRequestUpdate(CH.ifa.draw.framework.DrawingChangeEvent)</strong>: Update the drawing based on the given drawing change event.</p></li>
</ul>
</details>
<li><p><strong>Invalidate Drawing</strong>: Invalidate the drawing based on the given DrawingChangeEvent.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawingInvalidated(CH.ifa.draw.framework.DrawingChangeEvent)</strong>: Invalidate the drawing based on the given DrawingChangeEvent.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.framework.DrawingChangeEvent</strong>: Represents a drawing change event.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Retrieving invalidated rectangle</strong>: Return the rectangle that represents the area invalidated by the drawing change event.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getInvalidatedRectangle()</strong>: Return the rectangle that represents the area invalidated by the drawing change event.</p></li>
</ul>
</details>
<li><p><strong>Retrieving associated drawing</strong>: Return the drawing associated with this DrawingChangeEvent.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getDrawing()</strong>: Return the drawing associated with this DrawingChangeEvent.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>CH.ifa.draw.samples.javadraw</strong>: Open and manage a JavaDrawApp application.</p></li>
<details><summary>Subgoals:</summary>
<ul>
<li><p><strong>Drawing Management</strong>: Manage the drawing in the JavaDraw application</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.samples.javadraw.BouncingDrawing</strong>: This class represents a bouncing drawing that can add, replace, animate, and remove figures.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Adding Figures</strong>: Add a figure to the drawing, decorating it with animation if it is not already an animation decorator.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>add(CH.ifa.draw.framework.Figure)</strong>: Add a figure to the drawing, decorating it with animation if it is not already an animation decorator.</p></li>
</ul>
</details>
<li><p><strong>Replacing Figures</strong>: Replace a figure with a replacement figure, ensuring that the replacement is an instance of AnimationDecorator if it is not already.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>replace(CH.ifa.draw.framework.Figure,CH.ifa.draw.framework.Figure)</strong>: Replace a figure with a replacement figure, ensuring that the replacement is an instance of AnimationDecorator if it is not already.</p></li>
</ul>
</details>
<li><p><strong>Animating Figures</strong>: Animate each figure in the drawing by calling their animationStep() method.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>animationStep()</strong>: Animate each figure in the drawing by calling their `animationStep()` method.</p></li>
</ul>
</details>
<li><p><strong>Removing Figures</strong>: Remove the specified figure from the drawing and return the figure without the animation decorator.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>remove(CH.ifa.draw.framework.Figure)</strong>: Remove the specified figure from the drawing and return the figure without the animation decorator.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.samples.javadraw.JavaDrawViewer</strong>: Initialize and manage a viewer for JavaDraw, a drawing application.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Initialization</strong>: Initialize the JavaDrawViewer by setting the layout, creating the drawing view, adding it to the center, creating the follow URL tool, creating the icon kit, loading the drawing if a filename is provided, and displaying an error message if the drawing cannot be loaded.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>init()</strong>: Initialize the JavaDrawViewer by setting the layout, creating the drawing view, adding it to the center, creating the follow URL tool, creating the icon kit, loading the drawing if a filename is provided, and displaying an error message if the drawing cannot be loaded.</p></li>
</ul>
</details>
<li><p><strong>View Management</strong>: Return the drawing view of the JavaDrawViewer class.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>view()</strong>: Return the drawing view of the JavaDrawViewer class.</p></li>
</ul>
</details>
<li><p><strong>Tool Management</strong>: Return the tool used by the JavaDrawViewer class and finish the current tool operation.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>tool()</strong>: Return the tool used by the JavaDrawViewer class.</p></li>
<li><p><strong>toolDone()</strong>: Finish the current tool operation.</p></li>
</ul>
</details>
<li><p><strong>Drawing Management</strong>: Return the drawing associated with this JavaDrawViewer.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawing()</strong>: Return the drawing associated with this JavaDrawViewer.</p></li>
</ul>
</details>
<li><p><strong>Selection Management</strong>: Set the selected view of the JavaDrawViewer to the specified DrawingView.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>selectionChanged(CH.ifa.draw.framework.DrawingView)</strong>: Set the selected view of the JavaDrawViewer to the specified DrawingView.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Inspection</strong>: Open and inspect figures in the JavaDraw application</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.samples.javadraw.MySelectionTool</strong>: Open and inspect figures on mouse double-click, otherwise call superclass method.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Figure Inspection</strong>: Open the figure for inspection if the mouse is double-clicked</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseDown(java.awt.event.MouseEvent,int,int)</strong>: Open the figure for inspection if the mouse is double-clicked, otherwise call the superclass method.</p></li>
</ul>
</details>
<li><p><strong>Superclass Method Call</strong>: Call the superclass method if the mouse is not double-clicked</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseDown(java.awt.event.MouseEvent,int,int)</strong>: Open the figure for inspection if the mouse is double-clicked, otherwise call the superclass method.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Animation Control</strong>: Control the animation in the JavaDraw application</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.samples.javadraw.JavaDrawApplet</strong>: This class represents a JavaDrawApplet that can toggle animation on or off and start or end the animation.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Animation Control</strong>: Toggle animation on or off and start or end the animation.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>toggleAnimation()</strong>: Toggle the animation on or off depending on its current state.</p></li>
<li><p><strong>destroy()</strong>: Destroy the JavaDrawApplet by calling the superclass's destroy method and ending the animation.</p></li>
<li><p><strong>startAnimation()</strong>: Starts the animation of the JavaDrawApplet by creating a new Animator object and setting the label of the animation button to "End Animation".</p></li>
<li><p><strong>endAnimation()</strong>: Stop the animation and reset the animation button label.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.samples.javadraw.AnimationDecorator</strong>: Animate and control the movement of a decorator within a 300x300 box.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Set Velocity</strong>: Set the x and y velocities of the animation decorator.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>velocity(int,int)</strong>: Set the x and y velocities of the animation decorator.</p></li>
</ul>
</details>
<li><p><strong>Update Animation</strong>: Move the animation by updating its velocity and position based on its current speed and direction, while ensuring it stays within the bounds of a 300x300 box.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>animationStep()</strong>: Move the animation by updating its velocity and position based on its current speed and direction, while ensuring it stays within the bounds of a 300x300 box.</p></li>
</ul>
</details>
<li><p><strong>Read State</strong>: Read the state of the AnimationDecorator object from the given StorableInput.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the state of the AnimationDecorator object from the given StorableInput.</p></li>
</ul>
</details>
<li><p><strong>Set Display Box</strong>: Set the display box of the animation decorator using the given origin and corner points.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Set the display box of the animation decorator using the given origin and corner points.</p></li>
</ul>
</details>
<li><p><strong>Get Display Box</strong>: Return the display box of the AnimationDecorator class.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>displayBox()</strong>: Return the display box of the AnimationDecorator class.</p></li>
</ul>
</details>
<li><p><strong>Get Velocity</strong>: Return the velocity of the animation as a Point object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>velocity()</strong>: Return the velocity of the animation as a Point object.</p></li>
</ul>
</details>
<li><p><strong>Move Object</strong>: Move the object by the specified x and y coordinates.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>basicMoveBy(int,int)</strong>: Move the object by the specified x and y coordinates.</p></li>
</ul>
</details>
<li><p><strong>Write State</strong>: Write the x and y velocities of the AnimationDecorator object to the StorableOutput.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the x and y velocities of the AnimationDecorator object to the StorableOutput.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.samples.javadraw.Animator</strong>: Run and control an animation.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Animation Control</strong>: Start, stop, and control the animation.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>start()</strong>: Starts the animation by setting the `fIsRunning` flag to true.</p></li>
<li><p><strong>end()</strong>: Stop the animation.</p></li>
</ul>
</details>
<li><p><strong>Animation Execution</strong>: Run the animation by continuously updating the view, checking for damage, and delaying the execution.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>run()</strong>: Run the animation by continuously updating the view, checking for damage, and delaying the execution.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>URL Handling</strong>: Handle URLs associated with figures in the JavaDraw application</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.samples.javadraw.FollowURLTool</strong>: Handle mouse events to show and open URLs associated with figures.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Show URL</strong>: Show the URL of the figure if it exists, otherwise show an empty status.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseMove(java.awt.event.MouseEvent,int,int)</strong>: Show the URL of the figure if it exists, otherwise show an empty status.</p></li>
</ul>
</details>
<li><p><strong>Open URL</strong>: Open the URL associated with the clicked figure in a web browser.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseUp(java.awt.event.MouseEvent,int,int)</strong>: Open the URL associated with the clicked figure in a web browser.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.samples.javadraw.URLTool</strong>: This class is responsible for handling URL-related actions and editing in a drawing view.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Ending actions and editing</strong>: Ends the current action and stops editing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>endAction(java.awt.event.ActionEvent)</strong>: Ends the current action and stops editing.</p></li>
<li><p><strong>deactivate(CH.ifa.draw.framework.DrawingView)</strong>: Deactivates the URLTool and ends any ongoing editing in the specified DrawingView.</p></li>
</ul>
</details>
<li><p><strong>Handling mouse events</strong>: Handles the event when the mouse button is released at the specified coordinates and begins or ends editing based on mouse press.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseUp(java.awt.event.MouseEvent,int,int)</strong>: Handle the event when the mouse button is released at the specified coordinates.</p></li>
<li><p><strong>mouseDown(java.awt.event.MouseEvent,int,int)</strong>: Begin editing the figure if it is pressed, otherwise end the editing.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Application Management</strong>: Manage the JavaDrawApp application</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.samples.javadraw.JavaDrawApp</strong>: Open and manage a JavaDrawApp application.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Application Management</strong>: Open, start, and destroy the JavaDrawApp application.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>open()</strong>: Open the JavaDrawApp.</p></li>
<li><p><strong>startAnimation()</strong>: Starts the animation of the JavaDrawApp by creating a new Animator object and calling its start() method.</p></li>
<li><p><strong>destroy()</strong>: Destroy the JavaDrawApp by calling the superclass's destroy method and ending any ongoing animation.</p></li>
</ul>
</details>
<li><p><strong>View Management</strong>: Open and manage view windows for the JavaDrawApp application.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>openView()</strong>: Open a new view window for the JavaDrawApp application with the specified drawing and title.</p></li>
</ul>
</details>
<li><p><strong>Animation Management</strong>: Start and end animation for the JavaDrawApp application.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>startAnimation()</strong>: Starts the animation of the JavaDrawApp by creating a new Animator object and calling its start() method.</p></li>
<li><p><strong>endAnimation()</strong>: Ends the animation if it is currently running.</p></li>
</ul>
</details>
<li><p><strong>Main Window</strong>: Open the main JavaDrawApp window.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>main(java.lang.String[])</strong>: Open the JavaDrawApp window.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>View Management</strong>: Manage the view in the JavaDraw application</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.samples.javadraw.JavaDrawApp</strong>: Open and manage a JavaDrawApp application.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Application Management</strong>: Open, start, and destroy the JavaDrawApp application.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>open()</strong>: Open the JavaDrawApp.</p></li>
<li><p><strong>startAnimation()</strong>: Starts the animation of the JavaDrawApp by creating a new Animator object and calling its start() method.</p></li>
<li><p><strong>destroy()</strong>: Destroy the JavaDrawApp by calling the superclass's destroy method and ending any ongoing animation.</p></li>
</ul>
</details>
<li><p><strong>View Management</strong>: Open and manage view windows for the JavaDrawApp application.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>openView()</strong>: Open a new view window for the JavaDrawApp application with the specified drawing and title.</p></li>
</ul>
</details>
<li><p><strong>Animation Management</strong>: Start and end animation for the JavaDrawApp application.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>startAnimation()</strong>: Starts the animation of the JavaDrawApp by creating a new Animator object and calling its start() method.</p></li>
<li><p><strong>endAnimation()</strong>: Ends the animation if it is currently running.</p></li>
</ul>
</details>
<li><p><strong>Main Window</strong>: Open the main JavaDrawApp window.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>main(java.lang.String[])</strong>: Open the JavaDrawApp window.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.samples.javadraw.JavaDrawViewer</strong>: Initialize and manage a viewer for JavaDraw, a drawing application.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Initialization</strong>: Initialize the JavaDrawViewer by setting the layout, creating the drawing view, adding it to the center, creating the follow URL tool, creating the icon kit, loading the drawing if a filename is provided, and displaying an error message if the drawing cannot be loaded.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>init()</strong>: Initialize the JavaDrawViewer by setting the layout, creating the drawing view, adding it to the center, creating the follow URL tool, creating the icon kit, loading the drawing if a filename is provided, and displaying an error message if the drawing cannot be loaded.</p></li>
</ul>
</details>
<li><p><strong>View Management</strong>: Return the drawing view of the JavaDrawViewer class.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>view()</strong>: Return the drawing view of the JavaDrawViewer class.</p></li>
</ul>
</details>
<li><p><strong>Tool Management</strong>: Return the tool used by the JavaDrawViewer class and finish the current tool operation.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>tool()</strong>: Return the tool used by the JavaDrawViewer class.</p></li>
<li><p><strong>toolDone()</strong>: Finish the current tool operation.</p></li>
</ul>
</details>
<li><p><strong>Drawing Management</strong>: Return the drawing associated with this JavaDrawViewer.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawing()</strong>: Return the drawing associated with this JavaDrawViewer.</p></li>
</ul>
</details>
<li><p><strong>Selection Management</strong>: Set the selected view of the JavaDrawViewer to the specified DrawingView.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>selectionChanged(CH.ifa.draw.framework.DrawingView)</strong>: Set the selected view of the JavaDrawViewer to the specified DrawingView.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Animation Management</strong>: Manage the animation in the JavaDraw application</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.samples.javadraw.JavaDrawApp</strong>: Open and manage a JavaDrawApp application.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Application Management</strong>: Open, start, and destroy the JavaDrawApp application.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>open()</strong>: Open the JavaDrawApp.</p></li>
<li><p><strong>startAnimation()</strong>: Starts the animation of the JavaDrawApp by creating a new Animator object and calling its start() method.</p></li>
<li><p><strong>destroy()</strong>: Destroy the JavaDrawApp by calling the superclass's destroy method and ending any ongoing animation.</p></li>
</ul>
</details>
<li><p><strong>View Management</strong>: Open and manage view windows for the JavaDrawApp application.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>openView()</strong>: Open a new view window for the JavaDrawApp application with the specified drawing and title.</p></li>
</ul>
</details>
<li><p><strong>Animation Management</strong>: Start and end animation for the JavaDrawApp application.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>startAnimation()</strong>: Starts the animation of the JavaDrawApp by creating a new Animator object and calling its start() method.</p></li>
<li><p><strong>endAnimation()</strong>: Ends the animation if it is currently running.</p></li>
</ul>
</details>
<li><p><strong>Main Window</strong>: Open the main JavaDrawApp window.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>main(java.lang.String[])</strong>: Open the JavaDrawApp window.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Main Window</strong>: Manage the main window of the JavaDraw application</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.samples.javadraw.JavaDrawApp</strong>: Open and manage a JavaDrawApp application.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Application Management</strong>: Open, start, and destroy the JavaDrawApp application.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>open()</strong>: Open the JavaDrawApp.</p></li>
<li><p><strong>startAnimation()</strong>: Starts the animation of the JavaDrawApp by creating a new Animator object and calling its start() method.</p></li>
<li><p><strong>destroy()</strong>: Destroy the JavaDrawApp by calling the superclass's destroy method and ending any ongoing animation.</p></li>
</ul>
</details>
<li><p><strong>View Management</strong>: Open and manage view windows for the JavaDrawApp application.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>openView()</strong>: Open a new view window for the JavaDrawApp application with the specified drawing and title.</p></li>
</ul>
</details>
<li><p><strong>Animation Management</strong>: Start and end animation for the JavaDrawApp application.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>startAnimation()</strong>: Starts the animation of the JavaDrawApp by creating a new Animator object and calling its start() method.</p></li>
<li><p><strong>endAnimation()</strong>: Ends the animation if it is currently running.</p></li>
</ul>
</details>
<li><p><strong>Main Window</strong>: Open the main JavaDrawApp window.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>main(java.lang.String[])</strong>: Open the JavaDrawApp window.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Tool Management</strong>: Manage the tools in the JavaDraw application</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.samples.javadraw.JavaDrawViewer</strong>: Initialize and manage a viewer for JavaDraw, a drawing application.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Initialization</strong>: Initialize the JavaDrawViewer by setting the layout, creating the drawing view, adding it to the center, creating the follow URL tool, creating the icon kit, loading the drawing if a filename is provided, and displaying an error message if the drawing cannot be loaded.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>init()</strong>: Initialize the JavaDrawViewer by setting the layout, creating the drawing view, adding it to the center, creating the follow URL tool, creating the icon kit, loading the drawing if a filename is provided, and displaying an error message if the drawing cannot be loaded.</p></li>
</ul>
</details>
<li><p><strong>View Management</strong>: Return the drawing view of the JavaDrawViewer class.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>view()</strong>: Return the drawing view of the JavaDrawViewer class.</p></li>
</ul>
</details>
<li><p><strong>Tool Management</strong>: Return the tool used by the JavaDrawViewer class and finish the current tool operation.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>tool()</strong>: Return the tool used by the JavaDrawViewer class.</p></li>
<li><p><strong>toolDone()</strong>: Finish the current tool operation.</p></li>
</ul>
</details>
<li><p><strong>Drawing Management</strong>: Return the drawing associated with this JavaDrawViewer.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawing()</strong>: Return the drawing associated with this JavaDrawViewer.</p></li>
</ul>
</details>
<li><p><strong>Selection Management</strong>: Set the selected view of the JavaDrawViewer to the specified DrawingView.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>selectionChanged(CH.ifa.draw.framework.DrawingView)</strong>: Set the selected view of the JavaDrawViewer to the specified DrawingView.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Selection Management</strong>: Manage the selection of figures in the JavaDraw application</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.samples.javadraw.JavaDrawViewer</strong>: Initialize and manage a viewer for JavaDraw, a drawing application.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Initialization</strong>: Initialize the JavaDrawViewer by setting the layout, creating the drawing view, adding it to the center, creating the follow URL tool, creating the icon kit, loading the drawing if a filename is provided, and displaying an error message if the drawing cannot be loaded.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>init()</strong>: Initialize the JavaDrawViewer by setting the layout, creating the drawing view, adding it to the center, creating the follow URL tool, creating the icon kit, loading the drawing if a filename is provided, and displaying an error message if the drawing cannot be loaded.</p></li>
</ul>
</details>
<li><p><strong>View Management</strong>: Return the drawing view of the JavaDrawViewer class.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>view()</strong>: Return the drawing view of the JavaDrawViewer class.</p></li>
</ul>
</details>
<li><p><strong>Tool Management</strong>: Return the tool used by the JavaDrawViewer class and finish the current tool operation.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>tool()</strong>: Return the tool used by the JavaDrawViewer class.</p></li>
<li><p><strong>toolDone()</strong>: Finish the current tool operation.</p></li>
</ul>
</details>
<li><p><strong>Drawing Management</strong>: Return the drawing associated with this JavaDrawViewer.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>drawing()</strong>: Return the drawing associated with this JavaDrawViewer.</p></li>
</ul>
</details>
<li><p><strong>Selection Management</strong>: Set the selected view of the JavaDrawViewer to the specified DrawingView.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>selectionChanged(CH.ifa.draw.framework.DrawingView)</strong>: Set the selected view of the JavaDrawViewer to the specified DrawingView.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>CH.ifa.draw.samples.net</strong>: Open the NetApp window and represent a node in a network.</p></li>
<details><summary>Subgoals:</summary>
<ul>
<li><p><strong>Open NetApp window</strong>: The goal of this subgoal is to open the NetApp window of the DrawApplication class.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.samples.net.NetApp</strong>: Open the NetApp window of the DrawApplication class.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Open NetApp window</strong>: Open the NetApp window of the DrawApplication class.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>main(java.lang.String[])</strong>: Open the `NetApp` window of the `DrawApplication` class.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Represent a node in a network</strong>: The goal of this subgoal is to represent a node in a network using a figure.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.samples.net.NodeFigure</strong>: Represents a figure that represents a node in a network.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Connector Management</strong>: Manage the connectors of the node figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectorAt(int,int)</strong>: Return the connector at the specified coordinates.</p></li>
<li><p><strong>connectorVisibility(boolean)</strong>: Set the visibility of the connectors to the specified boolean value.</p></li>
</ul>
</details>
<li><p><strong>Handle Management</strong>: Manage the connection handles for the node figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Create and return a vector of connection handles for the node figure.</p></li>
</ul>
</details>
<li><p><strong>Drawing</strong>: Draw the node figure and its components.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws the node figure by calling the superclass's draw method, drawing the border, and drawing the connectors.</p></li>
</ul>
</details>
<li><p><strong>Display Box Calculation</strong>: Calculate and return the display box of the node figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>displayBox()</strong>: Calculate and return the display box of the NodeFigure with an increased size.</p></li>
</ul>
</details>
<li><p><strong>Point Containment Check</strong>: Check if given coordinates are contained within the visible connectors of the node figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>containsPoint(int,int)</strong>: Check if the given coordinates are contained within the visible connectors of the NodeFigure.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>CH.ifa.draw.samples.nothing</strong>: Open the NothingApp window of the DrawApplication class in the CH.ifa.draw.samples.nothing package.</p></li>
<details><summary>Subgoals:</summary>
<ul>
<li><p><strong>Open NothingApp window</strong>: Open the NothingApp window of the DrawApplication class</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.samples.nothing.NothingApp</strong>: Open the NothingApp window of the DrawApplication class.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Open window</strong>: Open the NothingApp window</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>main(java.lang.String[])</strong>: Open the `NothingApp` window of the `DrawApplication` class.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>CH.ifa.draw.samples.pert</strong>: Handle connections and dependencies between figures in a PERT diagram, open the Pert application, and represent figures in a PERT diagram with associated operations.</p></li>
<details><summary>Subgoals:</summary>
<ul>
<li><p><strong>Handle connections and dependencies between figures in a PERT diagram</strong>: This subgoal involves managing the connections and dependencies between figures in a PERT diagram.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.samples.pert.PertDependency</strong>: Handle connections and dependencies between figures in a PERT diagram.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Connection Handling</strong>: Handle the connection between two figures in the PERT diagram, checking for cycles and updating the figures accordingly.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handleConnect(CH.ifa.draw.framework.Figure,CH.ifa.draw.framework.Figure)</strong>: Handle the connection between two figures in the PERT diagram, checking for cycles and updating the figures accordingly.</p></li>
</ul>
</details>
<li><p><strong>Handle Management</strong>: Return a vector of handles for this PertDependency figure, including a null handle at the start.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Return a vector of handles for this PertDependency figure, including a null handle at the start.</p></li>
</ul>
</details>
<li><p><strong>Disconnection Handling</strong>: Disconnects the given start and end figures, removing the start figure as a pre-task of the end figure and updating the durations of the end figure, and removing the end figure as a post-task of the start figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handleDisconnect(CH.ifa.draw.framework.Figure,CH.ifa.draw.framework.Figure)</strong>: Disconnects the given start and end figures, removing the start figure as a pre-task of the end figure and updating the durations of the end figure, and removing the end figure as a post-task of the start figure.</p></li>
</ul>
</details>
<li><p><strong>Connection Validation</strong>: Check if both the start and end figures are instances of PertFigure in order to determine if a connection can be made.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>canConnect(CH.ifa.draw.framework.Figure,CH.ifa.draw.framework.Figure)</strong>: Check if both the start and end figures are instances of `PertFigure` in order to determine if a connection can be made.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Open the Pert application</strong>: This subgoal involves opening the Pert application.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.samples.pert.PertApplication</strong>: Open the Pert application.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Open Pert application</strong>: Open the Pert application.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>main(java.lang.String[])</strong>: Open the Pert application.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Represent a figure in a PERT diagram</strong>: This subgoal involves representing a figure in a PERT diagram and performing various operations related to it.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.samples.pert.PertFigure</strong>: Represents a figure in a PERT (Program Evaluation and Review Technique) diagram.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Task Management</strong>: Manage the pre and post tasks of the PertFigure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
</ul>
</details>
<li><p><strong>Duration Calculation</strong>: Calculate and update the duration of the PertFigure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>duration()</strong>: Calculate and return the duration of the PertFigure.</p></li>
<li><p><strong>updateDurations()</strong>: Update the end time of the PertFigure and notify any post tasks if the new end time is different from the current end time.</p></li>
<li><p><strong>start()</strong>: Calculate and return the earliest start time for the PertFigure by iterating through its pre-tasks and finding the maximum end time.</p></li>
<li><p><strong>end()</strong>: Return the end value of the PertFigure as an integer.</p></li>
</ul>
</details>
<li><p><strong>Layout and Display</strong>: Manage the layout and display of the PertFigure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectionInsets()</strong>: Return the insets for connecting to this PertFigure.</p></li>
<li><p><strong>notifyPostTasks()</strong>: Update the durations of the post tasks for the PertFigure.</p></li>
<li><p><strong>displayBox()</strong>: Return the display box of the PertFigure as a new Rectangle object.</p></li>
</ul>
</details>
<li><p><strong>Serialization</strong>: Read and write the state of the PertFigure object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
</ul>
</details>
<li><p><strong>Cycle Detection</strong>: Check for cycles in the dependencies of the PertFigure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
</ul>
</details>
<li><p><strong>Handle Creation</strong>: Create handles for the PertFigure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Create and return a vector of handles for the PertFigure class.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>CH.ifa.draw.standard</strong>: Provides a set of standard classes and interfaces for creating and manipulating figures in a drawing application.</p></li>
<details><summary>Subgoals:</summary>
<ul>
<li><p><strong>Handle Management</strong>: Create and manage handles for different corners and sides of a figure.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.standard.BoxHandleKit</strong>: Create and manage handles for different corners and sides of a figure.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Create handles for corners</strong>: Create handles representing the south-west, south-east, north-east, and north-west corners of a figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>southWest(CH.ifa.draw.framework.Figure)</strong>: Create a handle representing the south-west corner of the given figure.</p></li>
<li><p><strong>southEast(CH.ifa.draw.framework.Figure)</strong>: Create a handle representing the south-east corner of the given figure.</p></li>
<li><p><strong>northEast(CH.ifa.draw.framework.Figure)</strong>: Create and return a handle representing the north-east corner of the given figure.</p></li>
<li><p><strong>northWest(CH.ifa.draw.framework.Figure)</strong>: Create a handle for the northwest corner of the given figure.</p></li>
</ul>
</details>
<li><p><strong>Create handles for sides</strong>: Create handles representing the east, south, north, and west sides of a figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>east(CH.ifa.draw.framework.Figure)</strong>: Create and return a handle representing the eastern side of the given figure.</p></li>
<li><p><strong>south(CH.ifa.draw.framework.Figure)</strong>: Create a handle representing the south side of the given figure.</p></li>
<li><p><strong>north(CH.ifa.draw.framework.Figure)</strong>: Create and return a handle representing the north side of the given figure.</p></li>
<li><p><strong>west(CH.ifa.draw.framework.Figure)</strong>: Create a handle representing the western side of the given figure.</p></li>
</ul>
</details>
<li><p><strong>Add handles to figure</strong>: Add handles to a figure for each corner and for the north, south, east, and west sides.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>addHandles(CH.ifa.draw.framework.Figure,java.util.Vector)</strong>: Add handles to the given figure for each corner and for the north, south, east, and west sides.</p></li>
<li><p><strong>addCornerHandles(CH.ifa.draw.framework.Figure,java.util.Vector)</strong>: Add corner handles to the given figure and vector of handles.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Update Strategy</strong>: Draw the view onto the graphics object using a buffered update strategy.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.standard.BufferedUpdateStrategy</strong>: Draws the view onto the graphics object using a buffered update strategy.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Drawing</strong>: Draws the view onto the graphics object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics,CH.ifa.draw.framework.DrawingView)</strong>: Draws the view onto the graphics object using a buffered update strategy.</p></li>
</ul>
</details>
<li><p><strong>Update Strategy</strong>: Uses a buffered update strategy.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics,CH.ifa.draw.framework.DrawingView)</strong>: Draws the view onto the graphics object using a buffered update strategy.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Decoration</strong>: Add and remove decorations to a component figure.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>abstract class <strong>CH.ifa.draw.standard.DecoratorFigure</strong>: Represents a decorator figure that can add and remove decorations to a component figure.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Connection Insets</strong>: Return the connection insets of the decorator figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectionInsets()</strong>: Return the connection insets of the decorator figure.</p></li>
</ul>
</details>
<li><p><strong>Decoration Manipulation</strong>: Remove and retrieve the decoration from the figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>peelDecoration()</strong>: Remove the decoration from the figure and return it.</p></li>
</ul>
</details>
<li><p><strong>Connector Visibility</strong>: Set the visibility of the connectors for the decorator figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectorVisibility(boolean)</strong>: Set the visibility of the connectors for the decorator figure.</p></li>
</ul>
</details>
<li><p><strong>Attribute Manipulation</strong>: Retrieve and set attributes for the decorator figure's component.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getAttribute(java.lang.String)</strong>: Retrieve the attribute with the specified name from the decorator figure's component.</p></li>
<li><p><strong>setAttribute(java.lang.String,java.lang.Object)</strong>: Set the specified attribute with the given value for the decorator figure.</p></li>
</ul>
</details>
<li><p><strong>Figure Decomposition</strong>: Decompose the decorator figure into its component figures.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>decompose()</strong>: Decomposes the decorator figure into its component figures and returns an enumeration of them.</p></li>
</ul>
</details>
<li><p><strong>Figure Decoration</strong>: Add a figure to the container of the decorator figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>decorate(CH.ifa.draw.framework.Figure)</strong>: Add the given figure to the container of this decorator figure.</p></li>
</ul>
</details>
<li><p><strong>Figure Removal</strong>: Remove a figure from the decorator figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureRemoved(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the specified figure from the decorator figure.</p></li>
</ul>
</details>
<li><p><strong>Figure Serialization</strong>: Write the state of the decorator figure and its component to a StorableOutput object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the DecoratorFigure's state and its component to the given StorableOutput.</p></li>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads a `StorableInput` object and decorates the figure with the object read from it.</p></li>
</ul>
</details>
<li><p><strong>Connector Management</strong>: Return the connector at specified coordinates and update connector visibility.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectorAt(int,int)</strong>: Return the connector at the specified coordinates.</p></li>
</ul>
</details>
<li><p><strong>Figure Update</strong>: Update the figure request and notify listeners of changes.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureRequestUpdate(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the figure request by calling the figureRequestUpdate method of the listener if it is not null.</p></li>
<li><p><strong>figureInvalidated(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Notify the listener if the figure is invalidated.</p></li>
<li><p><strong>figureChanged(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the figure in response to a change event.</p></li>
<li><p><strong>figureRequestRemove(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the figure from the decorator figure if there is a listener present.</p></li>
</ul>
</details>
<li><p><strong>Figure Drawing</strong>: Draw the decorator figure and its component.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>draw(java.awt.Graphics)</strong>: Draws the decorator figure by calling the `draw` method of the component figure.</p></li>
</ul>
</details>
<li><p><strong>Figure Inclusion</strong>: Check if a figure is included in the decorator figure or its component.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>includes(CH.ifa.draw.framework.Figure)</strong>: Check if the given figure is included in the decorator figure or its component.</p></li>
</ul>
</details>
<li><p><strong>Figure Location</strong>: Find a figure inside the decorator figure at specified coordinates and move the decorator figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>findFigureInside(int,int)</strong>: Find the figure inside the decorator figure at the specified coordinates.</p></li>
<li><p><strong>moveBy(int,int)</strong>: Move the decorator figure by the specified x and y coordinates.</p></li>
</ul>
</details>
<li><p><strong>Figure Release</strong>: Release the decorator figure by removing it from the container and releasing its component.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>release()</strong>: Release the decorator figure by removing it from the container and releasing its component.</p></li>
</ul>
</details>
<li><p><strong>Figure Containment</strong>: Check if a given point is contained within the figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>containsPoint(int,int)</strong>: Check if the given point (x, y) is contained within the figure.</p></li>
</ul>
</details>
<li><p><strong>Figure Enumeration</strong>: Return an enumeration of the figures contained within the decorator figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figures()</strong>: Return an enumeration of the figures contained within the decorator figure.</p></li>
</ul>
</details>
<li><p><strong>Connected Text Locator</strong>: Return the locator for the connected text of a given figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>connectedTextLocator(CH.ifa.draw.framework.Figure)</strong>: Return the locator for the connected text of the given figure.</p></li>
</ul>
</details>
<li><p><strong>Display Box</strong>: Return the display box of the decorator figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>displayBox()</strong>: Return the display box of the decorator figure.</p></li>
<li><p><strong>basicDisplayBox(java.awt.Point,java.awt.Point)</strong>: Set the display box of the decorator figure using the given origin and corner points.</p></li>
</ul>
</details>
<li><p><strong>Component Handles</strong>: Return the handles of the component.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>handles()</strong>: Return the handles of the component.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Selecting Objects</strong>: Allow users to select an area on the canvas and perform actions based on the selected area.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.standard.SelectAreaTracker</strong>: SelectAreaTracker is a class that allows users to select an area on the canvas and perform actions based on the selected area.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Selecting an area</strong>: Selects an area on the canvas based on the mouse down event and the given coordinates.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseDown(java.awt.event.MouseEvent,int,int)</strong>: Selects an area on the canvas based on the mouse down event and the given coordinates.</p></li>
</ul>
</details>
<li><p><strong>Dragging the mouse</strong>: Drag the mouse to erase the rubber band and create a new rubber band from the anchor point to the current mouse position.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseDrag(java.awt.event.MouseEvent,int,int)</strong>: Drag the mouse to erase the rubber band and create a new rubber band from the anchor point to the current mouse position.</p></li>
</ul>
</details>
<li><p><strong>Selecting objects</strong>: Selects the group of objects within the specified area and removes the rubber band.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseUp(java.awt.event.MouseEvent,int,int)</strong>: Selects the group of objects within the specified area and removes the rubber band.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Manipulation</strong>: Perform actions on figures and interact with the editor.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>abstract class <strong>CH.ifa.draw.standard.ActionTool</strong>: Perform actions on figures and interact with the editor.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Perform actions on figures</strong>: Perform an action on the given figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>action(CH.ifa.draw.framework.Figure)</strong>: Perform an action on the given figure.</p></li>
</ul>
</details>
<li><p><strong>Interact with the editor</strong>: Selects the figure at the specified coordinates and adds it to the selection, then performs an action on the selected figure.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseDown(java.awt.event.MouseEvent,int,int)</strong>: Selects the figure at the specified coordinates and adds it to the selection, then performs an action on the selected figure.</p></li>
</ul>
</details>
<li><p><strong>Finish tool action and notify the editor</strong>: Finish the current tool action and notify the editor.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseUp(java.awt.event.MouseEvent,int,int)</strong>: Finish the current tool action and notify the editor.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Grid Constrain</strong>: Constrain points to a grid and provide information about the grid step sizes.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.standard.GridConstrainer</strong>: Constrains points to a grid and provides information about the grid step sizes.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Grid Constrain</strong>: Constrains points to the nearest grid point.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>constrainPoint(java.awt.Point)</strong>: Constrains the given point to the nearest grid point.</p></li>
</ul>
</details>
<li><p><strong>Grid Step Size</strong>: Returns the step size for the y-coordinate of the grid.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getStepY()</strong>: Return the step size for the y-coordinate of the grid.</p></li>
</ul>
</details>
<li><p><strong>Grid Step Size</strong>: Returns the step size in the x-direction for the grid constrainer.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getStepX()</strong>: Return the step size in the x-direction for the grid constrainer.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Change Notification</strong>: Manage and notify listeners of figure change events.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.standard.FigureChangeEventMulticaster</strong>: Manage and notify listeners of figure change events.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Figure Removal</strong>: Remove figures and notify listeners of the removal.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureRemoved(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the specified figure from the list of figures and notify all listeners that the figure has been removed.</p></li>
</ul>
</details>
<li><p><strong>Listener Management</strong>: Add and remove FigureChangeListeners from the multicaster.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>remove(CH.ifa.draw.framework.FigureChangeListener,CH.ifa.draw.framework.FigureChangeListener)</strong>: Remove the specified FigureChangeListener from the FigureChangeEventMulticaster.</p></li>
<li><p><strong>add(CH.ifa.draw.framework.FigureChangeListener,CH.ifa.draw.framework.FigureChangeListener)</strong>: Add a FigureChangeListener to the FigureChangeEventMulticaster.</p></li>
</ul>
</details>
<li><p><strong>Figure Change Notification</strong>: Notify listeners of figure changes and updates.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureChanged(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Notify all registered listeners that a figure has changed.</p></li>
<li><p><strong>figureRequestUpdate(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Update the figures in response to a figure change event.</p></li>
<li><p><strong>figureInvalidated(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Notify the listeners that a figure has been invalidated.</p></li>
</ul>
</details>
<li><p><strong>Event Removal</strong>: Remove figure change events from the list of listeners.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>figureRequestRemove(CH.ifa.draw.framework.FigureChangeEvent)</strong>: Remove the specified figure change event from the list of listeners.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Duplication</strong>: Duplicate selected figures in a view.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.standard.DuplicateCommand</strong>: Represents a command for duplicating selected figures in a view.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Checking if there is a selection</strong>: Check if there is a selection in the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>isExecutable()</strong>: Check if there is a selection in the view.</p></li>
</ul>
</details>
<li><p><strong>Executing the DuplicateCommand</strong>: Execute the DuplicateCommand by getting the figure selection from the view, clearing the selection, inserting the figures at coordinates (10, 10), and checking for any damage to the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>execute()</strong>: Execute the `DuplicateCommand` by getting the figure selection from the view, clearing the selection, inserting the figures at coordinates (10, 10), and checking for any damage to the view.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Alignment</strong>: Align selected figures in the view.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.standard.AlignCommand</strong>: AlignCommand class is responsible for aligning selected figures in the view.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Checking executability</strong>: Check if there are more than one selected objects in the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>isExecutable()</strong>: Check if there are more than one selected objects in the view.</p></li>
</ul>
</details>
<li><p><strong>Executing alignment</strong>: Aligns the selected figures based on the specified alignment option.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>execute()</strong>: Aligns the selected figures based on the specified alignment option.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Cut</strong>: Cut selected objects in a view.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.standard.CutCommand</strong>: This class represents a command for cutting selected objects in a view.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Checking if there is at least one item selected</strong>: Check if there is at least one item selected in the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>isExecutable()</strong>: Check if there is at least one item selected in the view.</p></li>
</ul>
</details>
<li><p><strong>Executing the cut command</strong>: Copy the selected objects, delete them, and update the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>execute()</strong>: Copy the selected objects, delete them, and update the view.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Copy</strong>: Copy selected items in the view.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.standard.CopyCommand</strong>: CopyCommand class is responsible for copying selected items in the view.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Copying</strong>: Copy the selected items.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>execute()</strong>: Copy the selected items.</p></li>
</ul>
</details>
<li><p><strong>Checking</strong>: Check if there is at least one selected item in the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>isExecutable()</strong>: Check if there is at least one selected item in the view.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Toggle Grid</strong>: Toggle the grid constrainer on or off for the view.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.standard.ToggleGridCommand</strong>: ToggleGridCommand toggles the grid constrainer on or off for the view.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Toggle grid constrainer</strong>: Toggle the grid constrainer on or off for the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>execute()</strong>: Toggle the grid constrainer on or off for the view.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Deletion</strong>: Delete selected objects and update the view.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.standard.DeleteCommand</strong>: DeleteCommand class is responsible for deleting selected objects and updating the view.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Checking if there is at least one selected item</strong>: Check if there is at least one selected item in the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>isExecutable()</strong>: Check if there is at least one selected item in the view.</p></li>
</ul>
</details>
<li><p><strong>Deleting selected objects and updating the view</strong>: Delete the selected objects and update the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>execute()</strong>: Delete the selected objects and update the view.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Bring to Front</strong>: Bring selected figures to the front of the drawing.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.standard.BringToFrontCommand</strong>: BringToFrontCommand class is responsible for bringing the selected figures to the front of the drawing.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Bringing figures to front</strong>: Bring the selected figures to the front of the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>execute()</strong>: Bring the selected figures to the front of the drawing.</p></li>
</ul>
</details>
<li><p><strong>Checking if there are selected objects</strong>: Check if there is at least one selected object in the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>isExecutable()</strong>: Check if there is at least one selected object in the view.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Send to Back</strong>: Move selected figures to the back of the drawing.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.standard.SendToBackCommand</strong>: Move selected figures to the back of the drawing.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Execute</strong>: Move the selected figures to the back of the drawing.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>execute()</strong>: Move the selected figures to the back of the drawing.</p></li>
</ul>
</details>
<li><p><strong>Check Executability</strong>: Check if there is at least one selected object in the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>isExecutable()</strong>: Check if there is at least one selected object in the view.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Paste</strong>: Paste figures from the clipboard into the view.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.standard.PasteCommand</strong>: Execute the paste command by retrieving the figures from the clipboard and inserting them into the view at the last clicked position.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Execute paste command</strong>: Retrieve figures from clipboard and insert them into the view at the last clicked position</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>execute()</strong>: Execute the paste command by retrieving the figures from the clipboard and inserting them into the view at the last clicked position.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Connection</strong>: Create and modify connections between figures.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.standard.ConnectionTool</strong>: This class is responsible for creating and modifying connections between figures.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Mouse interaction</strong>: Handle mouse events to create, modify, and remove connections.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseDrag(java.awt.event.MouseEvent,int,int)</strong>: Drag the mouse to update the position of the connection or the edited connection.</p></li>
<li><p><strong>deactivate()</strong>: Deactivates the connection tool and hides the target connector.</p></li>
<li><p><strong>mouseUp(java.awt.event.MouseEvent,int,int)</strong>: Connects the start and end connectors of a connection tool and updates the connection, or removes the connection if no target figure is found.</p></li>
<li><p><strong>mouseDown(java.awt.event.MouseEvent,int,int)</strong>: Create a connection between two figures or modify an existing connection based on the mouse down event.</p></li>
<li><p><strong>mouseMove(java.awt.event.MouseEvent,int,int)</strong>: Track the connectors of the connection tool based on the mouse movement.</p></li>
</ul>
</details>
<li><p><strong>Connection manipulation</strong>: Update the position and appearance of connections.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseDrag(java.awt.event.MouseEvent,int,int)</strong>: Drag the mouse to update the position of the connection or the edited connection.</p></li>
<li><p><strong>deactivate()</strong>: Deactivates the connection tool and hides the target connector.</p></li>
<li><p><strong>mouseUp(java.awt.event.MouseEvent,int,int)</strong>: Connects the start and end connectors of a connection tool and updates the connection, or removes the connection if no target figure is found.</p></li>
<li><p><strong>mouseDown(java.awt.event.MouseEvent,int,int)</strong>: Create a connection between two figures or modify an existing connection based on the mouse down event.</p></li>
<li><p><strong>mouseMove(java.awt.event.MouseEvent,int,int)</strong>: Track the connectors of the connection tool based on the mouse movement.</p></li>
</ul>
</details>
<li><p><strong>Connector tracking</strong>: Track the connectors of the connection tool based on mouse movement.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseDrag(java.awt.event.MouseEvent,int,int)</strong>: Drag the mouse to update the position of the connection or the edited connection.</p></li>
<li><p><strong>deactivate()</strong>: Deactivates the connection tool and hides the target connector.</p></li>
<li><p><strong>mouseUp(java.awt.event.MouseEvent,int,int)</strong>: Connects the start and end connectors of a connection tool and updates the connection, or removes the connection if no target figure is found.</p></li>
<li><p><strong>mouseDown(java.awt.event.MouseEvent,int,int)</strong>: Create a connection between two figures or modify an existing connection based on the mouse down event.</p></li>
<li><p><strong>mouseMove(java.awt.event.MouseEvent,int,int)</strong>: Track the connectors of the connection tool based on the mouse movement.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Figure Attribute Change</strong>: Change the attribute of selected figures in the view.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.standard.ChangeAttributeCommand</strong>: Represents a command to change the attribute of selected figures in the view.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Checking executability</strong>: Check if there is at least one selected object in the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>isExecutable()</strong>: Check if there is at least one selected object in the view.</p></li>
</ul>
</details>
<li><p><strong>Executing attribute change</strong>: Set the attribute of the selected figures to the specified value and update the view.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>execute()</strong>: Set the attribute of the selected figures to the specified value and update the view.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>CH.ifa.draw.util</strong>: Provides utility classes and interfaces for handling palette buttons, geometric calculations, command choices, palette events, layout management, command menus, fillers, commands, color manipulation, image loading, data storage, animation, clipboard management, text fields, vector iteration, and command buttons.</p></li>
<details><summary>Subgoals:</summary>
<ul>
<li><p><strong>Palette Button Management</strong>: Handle the behavior and visual state of palette buttons.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>abstract class <strong>CH.ifa.draw.util.PaletteButton</strong>: Handle the behavior and visual state of a palette button.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Mouse Events</strong>: Handle mouse events such as mouseExited, mouseClicked, mouseMoved, mouseReleased, mouseEntered, mousePressed, mouseDragged.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>mouseExited(java.awt.event.MouseEvent)</strong>: Handle the event when the mouse exits the button by calling the `mouseDragged` method if the button is pressed and notifying the listener that the user is no longer over the palette button.</p></li>
<li><p><strong>mouseClicked(java.awt.event.MouseEvent)</strong>: Handle the mouse click event.</p></li>
<li><p><strong>mouseMoved(java.awt.event.MouseEvent)</strong>: Set the palette user over state to true when the mouse is moved.</p></li>
<li><p><strong>mouseReleased(java.awt.event.MouseEvent)</strong>: Set the button state to its previous state, repaint the button, and notify the listener if the mouse is released within the button's bounds.</p></li>
<li><p><strong>mouseEntered(java.awt.event.MouseEvent)</strong>: Set the behavior when the mouse enters the component.</p></li>
<li><p><strong>mousePressed(java.awt.event.MouseEvent)</strong>: Set the state of the button to "pressed" and repaint it.</p></li>
<li><p><strong>mouseDragged(java.awt.event.MouseEvent)</strong>: Set the state of the button to "pressed" if the mouse is within the button's boundaries, otherwise set it to the previous state.</p></li>
</ul>
</details>
<li><p><strong>Painting</strong>: Paint the button in different visual states using the specified graphics context.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>paintPressed(java.awt.Graphics)</strong>: Paints the button in a pressed state using the specified graphics context.</p></li>
<li><p><strong>paintBackground(java.awt.Graphics)</strong>: Paints the background of the palette button using the specified graphics context.</p></li>
<li><p><strong>paintSelected(java.awt.Graphics)</strong>: Paints the selected state of the palette button using the specified graphics context.</p></li>
<li><p><strong>paintNormal(java.awt.Graphics)</strong>: Paints the button in its normal state using the specified graphics context.</p></li>
<li><p><strong>paint(java.awt.Graphics)</strong>: Paints the button with the appropriate visual style based on its state.</p></li>
</ul>
</details>
<li><p><strong>Button State</strong>: Handle the state of the button such as select, reset, value.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>select()</strong>: Selects the palette button and updates its visual state.</p></li>
<li><p><strong>reset()</strong>: Reset the state of the palette button to normal and repaint it.</p></li>
<li><p><strong>value()</strong>: Return the value of the PaletteButton.</p></li>
</ul>
</details>
<li><p><strong>Update Graphics</strong>: Update the graphics of the palette button by calling the paint method.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>update(java.awt.Graphics)</strong>: Update the graphics of the palette button by calling the paint method.</p></li>
</ul>
</details>
<li><p><strong>Button Name</strong>: Return the name of the palette button.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>name()</strong>: Return the name of the palette button.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>interface <strong>CH.ifa.draw.util.PaletteListener</strong>: Represents a listener for palette events.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Button state management</strong>: Set the state of the button to indicate whether the user is currently hovering over it or not.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>paletteUserOver(CH.ifa.draw.util.PaletteButton,boolean)</strong>: Set the state of the button to indicate whether the user is currently hovering over it or not.</p></li>
</ul>
</details>
<li><p><strong>Palette button selection</strong>: Open the selected palette button.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>paletteUserSelected(CH.ifa.draw.util.PaletteButton)</strong>: Open the selected palette button.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Geometric Calculations</strong>: Perform geometric calculations and operations on shapes.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.util.Geom</strong>: Calculate geometric properties and perform operations on shapes.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Point Operations</strong>: Perform operations on points such as calculating the west, east, south, north, and center points of a rectangle.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>west(java.awt.Rectangle)</strong>: Return the point on the west side of the given rectangle.</p></li>
<li><p><strong>east(java.awt.Rectangle)</strong>: Return the point at the east side of the given rectangle.</p></li>
<li><p><strong>south(java.awt.Rectangle)</strong>: Return the point at the center of the bottom edge of the given rectangle.</p></li>
<li><p><strong>north(java.awt.Rectangle)</strong>: Return the point at the top center of the given rectangle.</p></li>
<li><p><strong>center(java.awt.Rectangle)</strong>: Calculate and return the center point of the given rectangle.</p></li>
</ul>
</details>
<li><p><strong>Angle and Polar Coordinates</strong>: Calculate coordinates and angles based on given angles and polar coordinates.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>angleToPoint(java.awt.Rectangle,double)</strong>: Calculate the coordinates of a point on the given rectangle based on the specified angle.</p></li>
<li><p><strong>ovalAngleToPoint(java.awt.Rectangle,double)</strong>: Calculate the coordinates of a point on the circumference of an oval given its angle and the oval's bounding rectangle.</p></li>
<li><p><strong>polarToPoint(double,double,double)</strong>: Converts polar coordinates to Cartesian coordinates and returns a new Point object.</p></li>
<li><p><strong>pointToAngle(java.awt.Rectangle,java.awt.Point)</strong>: Calculate the angle between a given rectangle and point.</p></li>
</ul>
</details>
<li><p><strong>Line Operations</strong>: Perform operations on lines such as checking if a line contains a point, calculating the direction between two points, and calculating the intersection point between two line segments.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>lineContainsPoint(int,int,int,int,int,int)</strong>: Check if a line contains a given point within a certain tolerance.</p></li>
<li><p><strong>direction(int,int,int,int)</strong>: Calculate the direction between two points.</p></li>
<li><p><strong>intersect(int,int,int,int,int,int,int,int)</strong>: Calculate the intersection point between two line segments given their coordinates.</p></li>
</ul>
</details>
<li><p><strong>Value and Length Operations</strong>: Perform operations on values and lengths such as limiting a value within a specified range and calculating the length of a line segment.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>range(int,int,int)</strong>: Limit the given value to be within the specified range.</p></li>
<li><p><strong>length2(int,int,int,int)</strong>: Calculate the square of the length between two points given their coordinates.</p></li>
<li><p><strong>length(int,int,int,int)</strong>: Calculate the length of a line segment given its coordinates.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Command Management</strong>: Manage command choices, menus, and execution.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.util.CommandChoice</strong>: Represents a command choice and provides methods to add commands and execute the selected command.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Adding commands</strong>: Add a command to the command choice and update the list of commands.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>addItem(CH.ifa.draw.util.Command)</strong>: Add a command to the command choice and update the list of commands.</p></li>
</ul>
</details>
<li><p><strong>Executing selected command</strong>: Execute the selected command when the item state changes.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>itemStateChanged(java.awt.event.ItemEvent)</strong>: Execute the selected command when the item state changes.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.util.CommandMenu</strong>: Manage a command menu and its associated commands.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Add and Remove Commands</strong>: Add or remove commands from the command menu.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>add(CH.ifa.draw.util.Command)</strong>: Add a command to the command menu and associate it with a menu item.</p></li>
<li><p><strong>remove(CH.ifa.draw.util.Command)</strong>: Remove the specified command from the command menu.</p></li>
<li><p><strong>remove(java.awt.MenuItem)</strong>: Remove the specified menu item from the command menu.</p></li>
</ul>
</details>
<li><p><strong>Enable and Disable Menu Items</strong>: Enable or disable menu items based on the executability of the corresponding commands.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>enable(java.lang.String,boolean)</strong>: Enable or disable a menu item with the specified name.</p></li>
<li><p><strong>checkEnabled()</strong>: Check the enabled status of the menu items based on the executability of the corresponding commands.</p></li>
</ul>
</details>
<li><p><strong>Execute Selected Command</strong>: Execute the command associated with the selected menu item.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>actionPerformed(java.awt.event.ActionEvent)</strong>: Execute the command associated with the selected menu item.</p></li>
</ul>
</details>
<li><p><strong>Add Command with Shortcut</strong>: Add a new command to the command menu with the specified shortcut.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>add(CH.ifa.draw.util.Command,java.awt.MenuShortcut)</strong>: Add a new command to the command menu with the specified shortcut.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>abstract class <strong>CH.ifa.draw.util.Command</strong>: Represents a command that can be executed.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Retrieve command information</strong>: Return the name of the command.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>name()</strong>: Return the name of the command.</p></li>
</ul>
</details>
<li><p><strong>Execute command</strong>: Execute the command.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>execute()</strong>: Execute the command.</p></li>
</ul>
</details>
<li><p><strong>Check command executability</strong>: Check if the command is executable.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>isExecutable()</strong>: Check if the command is executable.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.util.CommandButton</strong>: Execute the command associated with this button and update the button label if necessary.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Execute command</strong>: Execute the command associated with this button.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>actionPerformed(java.awt.event.ActionEvent)</strong>: Execute the command associated with this button and update the button label if necessary.</p></li>
</ul>
</details>
<li><p><strong>Update button label</strong>: Update the button label if necessary.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>actionPerformed(java.awt.event.ActionEvent)</strong>: Execute the command associated with this button and update the button label if necessary.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Layout Management</strong>: Layout components in a container according to specified parameters.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.util.PaletteLayout</strong>: Layouts components in a container according to specified parameters.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Layouting</strong>: Layouts the components in the specified container according to the specified border, vertical layout flag, and gap.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>layoutContainer(java.awt.Container)</strong>: Layouts the components in the specified container according to the specified border, vertical layout flag, and gap.</p></li>
</ul>
</details>
<li><p><strong>Component Management</strong>: Add, remove, and manage components in the layout.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>addLayoutComponent(java.lang.String,java.awt.Component)</strong>: Add a component to the layout with the specified name.</p></li>
<li><p><strong>removeLayoutComponent(java.awt.Component)</strong>: Remove the specified component from the layout.</p></li>
</ul>
</details>
<li><p><strong>Size Calculation</strong>: Calculate and return the minimum and preferred layout size of the given container.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>minimumLayoutSize(java.awt.Container)</strong>: Calculate and return the minimum size of the layout for the given container.</p></li>
<li><p><strong>preferredLayoutSize(java.awt.Container)</strong>: Calculate and return the preferred layout size of the given container.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Filler Management</strong>: Manage fillers in a drawing application.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.util.Filler</strong>: Represents a utility class for managing fillers in a drawing application.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Size management</strong>: Manage the size of the Filler object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getMinimumSize()</strong>: Return the minimum size of the Filler object as a java.awt.Dimension.</p></li>
<li><p><strong>getPreferredSize()</strong>: Return the preferred size of the Filler component.</p></li>
</ul>
</details>
<li><p><strong>Background color management</strong>: Manage the background color of the filler.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getBackground()</strong>: Return the background color of the filler, or the default background color if none is set.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Color Manipulation</strong>: Manipulate and retrieve colors from a color map.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.util.ColorMap</strong>: This class provides a color map and various methods to manipulate and retrieve colors from the map.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Color Manipulation</strong>: Methods to manipulate and retrieve colors from the color map.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>colorIndex(java.awt.Color)</strong>: Return the index of the given color in the color map.</p></li>
<li><p><strong>isTransparent(java.awt.Color)</strong>: Check if the given color is transparent.</p></li>
<li><p><strong>name(int)</strong>: Return the name of the color at the specified index in the ColorMap array.</p></li>
<li><p><strong>color(java.lang.String)</strong>: Return the color associated with the given name, or black if no color is found.</p></li>
<li><p><strong>size()</strong>: Return the size of the ColorMap.</p></li>
<li><p><strong>color(int)</strong>: Return the color at the specified index in the ColorMap array, or throw an exception if the index is out of bounds.</p></li>
</ul>
</details>
<li><p><strong>Exception Handling</strong>: Method to handle index out of bounds exception.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>color(int)</strong>: Return the color at the specified index in the ColorMap array, or throw an exception if the index is out of bounds.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Image Loading</strong>: Load and cache images.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.util.Iconkit</strong>: This class provides utility methods for loading and caching images.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Image Loading</strong>: Load and cache images from files or resources.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>loadImage(java.lang.String)</strong>: Load an image from a file or resource and return it, caching it if necessary.</p></li>
<li><p><strong>loadImageResource(java.lang.String)</strong>: Load an image resource from the specified resource name using the default toolkit and return the loaded image.</p></li>
<li><p><strong>registerAndLoadImage(java.awt.Component,java.lang.String)</strong>: Register and load an image for a given component using the specified file name.</p></li>
<li><p><strong>getImage(java.lang.String)</strong>: Load and return an image based on the given filename, or load registered images and return the image if it exists.</p></li>
<li><p><strong>loadRegisteredImages(java.awt.Component)</strong>: Load and register images for a given component using a media tracker.</p></li>
<li><p><strong>registerImage(java.lang.String)</strong>: Register an image file with the Iconkit class.</p></li>
</ul>
</details>
<li><p><strong>Instance Management</strong>: Return an instance of the Iconkit class.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>instance()</strong>: Return an instance of the Iconkit class.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Data Storage</strong>: Write and read objects to/from input/output streams.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.util.StorableOutput</strong>: Write and store various data types to an output stream.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Writing double values</strong>: Write a double value to the output stream and add a space after it.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>writeDouble(double)</strong>: Write the double value to the output stream and add a space after it.</p></li>
</ul>
</details>
<li><p><strong>Writing color values</strong>: Write the RGB values of a given color to the output stream.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>writeColor(java.awt.Color)</strong>: Write the RGB values of the given color to the output stream.</p></li>
</ul>
</details>
<li><p><strong>Writing boolean values</strong>: Write a boolean value to the output stream.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>writeBoolean(boolean)</strong>: Write a documentation comment that explains that this method writes a boolean value to the output stream.</p></li>
</ul>
</details>
<li><p><strong>Writing string values</strong>: Write a given string to the output stream, escaping special characters.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>writeString(java.lang.String)</strong>: Write a documentation comment for the `writeString` method that explains how it writes a given string to the output stream, escaping special characters.</p></li>
</ul>
</details>
<li><p><strong>Closing the output stream</strong>: Close the output stream.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>close()</strong>: Close the output stream.</p></li>
</ul>
</details>
<li><p><strong>Writing storable objects</strong>: Write a storable object to the output stream.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>writeStorable(CH.ifa.draw.util.Storable)</strong>: Write a documentation comment that describes the purpose and behavior of the `writeStorable` method in imperative mood.</p></li>
</ul>
</details>
<li><p><strong>Writing integer values</strong>: Write an integer value to the output stream and add a space after it.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>writeInt(int)</strong>: Write an integer value to the output stream and add a space after it.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>class <strong>CH.ifa.draw.util.StorableInput</strong>: Reads and retrieves various types of data from an input stream.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Color reading</strong>: Reads the RGB values from the input stream and returns a new Color object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>readColor()</strong>: Reads the RGB values from the input stream and returns a new Color object.</p></li>
</ul>
</details>
<li><p><strong>Boolean reading</strong>: Reads a boolean value from the input stream and returns it, throwing an exception if an integer is not found.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>readBoolean()</strong>: Reads a boolean value from the input stream and returns it, throwing an exception if an integer is not found.</p></li>
</ul>
</details>
<li><p><strong>Double reading</strong>: Reads a double value from the input stream and returns it, or throws an IOException if a double value is not found.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>readDouble()</strong>: Reads a double value from the input stream and returns it, or throws an IOException if a double value is not found.</p></li>
</ul>
</details>
<li><p><strong>String reading</strong>: Reads and returns a string from the input, throwing an IOException if a string is not found.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>readString()</strong>: Reads and returns a string from the input, throwing an IOException if a string is not found.</p></li>
</ul>
</details>
<li><p><strong>Storable object reading</strong>: Reads a storable object from the input stream and returns it.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>readStorable()</strong>: Reads a storable object from the input stream and returns it.</p></li>
</ul>
</details>
<li><p><strong>Integer reading</strong>: Reads and returns an integer value from the input, throwing an exception if the input is not an integer.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>readInt()</strong>: Reads and returns an integer value from the input, throwing an exception if the input is not an integer.</p></li>
</ul>
</details>
</ul>
</details>
<li><p>interface <strong>CH.ifa.draw.util.Storable</strong>: Write and read objects to/from input/output streams.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Serialization</strong>: Write and read objects to/from input/output streams.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>write(CH.ifa.draw.util.StorableOutput)</strong>: Write the given `StorableOutput` object to the output stream.</p></li>
<li><p><strong>read(CH.ifa.draw.util.StorableInput)</strong>: Reads the object from the specified input stream.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Animation</strong>: Perform animation steps.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>interface <strong>CH.ifa.draw.util.Animatable</strong>: Perform animation steps.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Animation</strong>: Perform a single step in the animation.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>animationStep()</strong>: Perform a single step in the animation.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Clipboard Management</strong>: Manage the clipboard contents.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.util.Clipboard</strong>: Manage the clipboard contents.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Set contents</strong>: Set the contents of the clipboard to the specified object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>setContents(java.lang.Object)</strong>: Set the contents of the clipboard to the specified object.</p></li>
</ul>
</details>
<li><p><strong>Get contents</strong>: Return the contents of the clipboard.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getContents()</strong>: Return the contents of the clipboard.</p></li>
</ul>
</details>
<li><p><strong>Get clipboard</strong>: Return the clipboard object.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getClipboard()</strong>: Return the clipboard object.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Floating Text Field Overlay</strong>: Manage floating text fields overlayed on a container.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.util.FloatingTextField</strong>: Represents a floating text field that can be overlayed on a container.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Overlay Management</strong>: Manage the overlay of the floating text field.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>endOverlay()</strong>: Ends the overlay of the floating text field by hiding the edit widget, removing it from the container, and repainting the container.</p></li>
<li><p><strong>createOverlay(java.awt.Container)</strong>: Create an overlay for the specified container with the option to provide a custom text field.</p></li>
<li><p><strong>createOverlay(java.awt.Container,java.awt.Font)</strong>: Create an overlay for the specified container with the given font.</p></li>
</ul>
</details>
<li><p><strong>Text Field Manipulation</strong>: Manipulate the text field and its properties.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>getPreferredSize(int)</strong>: Return the preferred size of the text field based on the specified number of columns.</p></li>
<li><p><strong>removeActionListener(java.awt.event.ActionListener)</strong>: Remove the specified ActionListener from the FloatingTextField's edit widget.</p></li>
<li><p><strong>addActionListener(java.awt.event.ActionListener)</strong>: Add an ActionListener to the FloatingTextField.</p></li>
<li><p><strong>setBounds(java.awt.Rectangle,java.lang.String)</strong>: Set the bounds of the floating text field and display the specified text.</p></li>
<li><p><strong>getText()</strong>: Return the text entered in the floating text field.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
<li><p><strong>Vector Iteration</strong>: Iterate over a vector in reverse order.</p></li>
<details><summary>Classes involved:</summary>
<ul>
<li><p>class <strong>CH.ifa.draw.util.ReverseVectorEnumerator</strong>: ReverseVectorEnumerator class provides a way to iterate over a vector in reverse order.</p></li>
<details><summary>Class responsibilities:</summary>
<ul>
<li><p><strong>Iterating over vector</strong>: Return the next element in the vector in reverse order.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>nextElement()</strong>: Return the next element in the vector in reverse order.</p></li>
</ul>
</details>
<li><p><strong>Checking for more elements</strong>: Check if there are more elements in the reverse vector enumerator.</p></li>
<details><summary>Methods involved:</summary>
<ul>
<li><p><strong>hasMoreElements()</strong>: Check if there are more elements in the reverse vector enumerator.</p></li>
</ul>
</details>
</ul>
</details>
</ul>
</details>
</ul>
</details>
</ul>