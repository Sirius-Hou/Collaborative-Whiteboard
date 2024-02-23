## Problem

- The goal is to solve the problem of remote, visual collaboration by offering a platform for sketching, diagramming, and sharing ideas in real-time.
- Creating a real-time multi-user whiteboard tailored for professionals like students, designers, developers, and architects to make learning and brainstorming processes interactive and collaborative in a remote setting

## Users

- Tutors/TAs
- Remote software development teams focused on system architecture and design
- Persona and Interview Feedback:  

>>>
**Persona: John the Math Tutor**

Bio: John is a 3rd year student in University of Waterloo, majoring in Mathematics/Teaching. As a side hobby, he helps other students out on their math problems at the Math Tutoring Centre in the Math and Computer building. He is passionate about spreading knowledge, and will do anything to make his teaching more engaging. He is open to use new technologies. 

Goals: Make students understand concepts quickly. Make teaching interesting.

Frustrations: Poor engagement when teaching students in virtual meetings. Cannot communicate clearly to students online.

Motivations (1-5): 
    Incentive: 5,
    Fear: 1,
    Achievement: 2,
    Growth: 1,
    Social: 3,

Age: 21

Occupation: Student

Personality: friendly, patient

Quote: Nothing beats the simple whiteboard and marker.
>>>



>>>
**Interview feedback**

I contacted a data science intern, and according to their feedback, the proposed virtual whiteboard application could greatly simplify discussions involving graphs and other flowcharts within the team. Currently, they are compelled to meet in person once a week, during which the manager crudely sketches concepts on the physical office whiteboard or relies on Excel features, which is not an optimal solution. The ability to address doubts in real-time would significantly enhance their efficiency. 
One prominent feature they emphasized they would want is the capacity to import PDF files and download annotated notes, even if you're not the session host. They expressed overall enthusiasm for this idea and indicated their willingness to use it. However, their only concern revolved around the necessity of purchasing a stylus or pencil for effective use of the application. They weren't entirely certain about the feasibility of complete freehand drawing.

Furthermore, I reached out to several tutors, and they expressed the view that a virtual whiteboard could be a valuable tool, particularly in remote teaching scenarios. They believe that certain complex topics are challenging to convey through text alone, and having a visual representation would enhance comprehension for both themselves and their students.

In terms of specific features, they expressed the desire for a variety of backgrounds for the whiteboard to create a more immersive notebook or graph-like experience. A crucial requirement for them is that the application should be highly responsive to ensure that users do not encounter any delays, as this is vital for synchronized learning.

Tutors also highlighted their interest in the ability to grant access control, enabling selective students to contribute and write on the whiteboard to explain their queries, replicating a classroom experience. Additionally, they saw the potential for this app to serve as an icebreaker, allowing for informal drawing games like Pictionary to foster a cohesive virtual class environment.
>>>

## Major (Functional) Requirements

- Completed Requirements:
    - High Priority/Core features:
        - Basic canvas to sketch (#15, #1, #26) 
        - Support different strokes (thickness) and colors (#2, #16)
        - Eraser which can be resized (#3, #25), Button to clear entire canvas (#21)
        - Undo/Redo: Implement undo and redo functionality (#4, #42)
        - Real-time Collaboration: Synchronize canvas across multiple users in real-time (#22, #23, #30, #31, #32, #33, #39, #40)
        - Import a photo and edit on it (#28)
        - Export canvas as pdf (#27)
        - Zoom (#41) and drag (#20) on canvas 

    - Low Priority/Additional Requirements:
        - Preformed Shapes: Provide a library of shapes like rectangles, circles, and straight lines (#8)
        - Be able to move shapes (#19)
        - Dark mode (#10)


- Incomplete/Dropped Requirements
    - High Priority/Core features:
        - Implement user registration and login (this was dropped after deciding to use session ids to join sessions; #14)
        - Save canvas as a file and be able to load it back later (this was done in issue #17 but dropped after deciding to take a remote storage approach) 
        - Import pdf
        - Export as image
        - Access Control: Role-based permissions for editing and viewing (this was dropped after deciding to use sessions ids and not user login/registration since it did not seem appropriate; #11)
     
    - Low Priority/Additional Requirements:
        - Resizing shapes
        - Shape Connections: Enable lines to connect different shapes, forming diagrams
        - Text Annotation: Allow text to be added to shapes or directly on the canvas
        - Customizable background (lines/college-ruled, or) (this was supported by allowing users to import an image as a background, #9)
        - Version History: Track and revert to previous versions of the canvas (this was dropped since it did not seem as important after implementing undo/redo and considering the limited time, #12)

**Note:** Any feature above not dropped was incomplete due to lack of time and having to prioritize other features. Priority was given based on the value of the feature to the target users and time required as well as the complexity of implementing the feature.