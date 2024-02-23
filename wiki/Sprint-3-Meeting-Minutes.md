People present: Sirius, Akshita, Sohaib, David

UI/Whiteboard:
- Change eraser's behavior to delete entire shape (Sirius)
    - design issue: should erasing on rectangle erase the entire rectangle?
    - change will address another issue: dragging shape after erasing doesn't work
- Issue: No option to tap when drawing right now (Sirius)
    - fix will also require adding a shape-select button to select and drag shapes
- Exporting as image/pdf (Akshita)
- Zoom and drag on canvas (Akshita)
- Import image/pdf (undecided/together)
- Issue: eraser creates white lines, won't work on custom backgrounds (undecided/together)
    - needs to be address for task above (import image/pdf)
- UI for creating sessions, joining old sessions (Sohaib+David)

Other:
- Continue work on Server/Client communication (Sohaib+David): 
	- Enhance APIs further and address bugs (multiple devices drawing together is buggy, duplicate objects being sent, color not supported, drawing too quick causes loss of objects)
	- Support syncing with other actions on whiteboard like shape dragging, undo/redo, etc.
	- Reduce syncing latency (currently very slow)
	- Support multiple sessions and add mechanism to create/join sessions (such as links/sessions ids)
	- Setup database on server to store all objects
- Restructuring of project (Sohaib)
    - separate files for ui/presentation, business logic, and apis to communicate with web service
    - can follow a design pattern like MVVM
- File to store server's ip address (Sohaib+David)
    - to allow adjusting server's ip  address without rebuilding project

Low priority:
- Resizing shapes
- Sharing exported files
- Bug in shape drawing (object is not drawn where it is supposed)
- Canvas resizing issue (rotating does not preserve location of drawn objects)
- General ui/visual improvements and bug fixes:
    * problem: thickness slider too close to edge of screen
    * add extra vertical spacing above and below color buttons in toolbar
    * problem: toolbar not entirely at the bottom on physical device
- Performance improvements for whiteboard and drawing:
    - Affects responsiveness of app (if app gets too slow, drawings become less smooth)
    - Undo/redo can be made more memory/runtime efficient