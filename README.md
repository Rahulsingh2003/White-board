# White-board

Your **Whiteboard Drawing App** has several key functionalities, covering drawing, collaboration, sticky notes, image handling, and real-time updates. Below is a detailed breakdown of **all** its features.

---

## **🎨 Core Functionalities**
### **1️⃣ Drawing Tools**
✔ **Pencil Tool:** Allows freehand drawing with configurable color and thickness.  
✔ **Eraser Tool:** Erases drawn content by setting `globalCompositeOperation = "destination-out"`.  
✔ **Size Adjustment:** Users can change the thickness of the pencil/eraser.  

### **2️⃣ Undo & Redo System**
✔ **Undo:** Removes the last drawn action by popping from `undoStack` and pushing to `redoStack`.  
✔ **Redo:** Restores the last undone action from `redoStack`.  
✔ **Real-time Sync:** Undo/Redo actions are broadcasted across all users.  

---

## **📝 Sticky Notes System**
✔ **Create Sticky Notes:** Users can create movable and resizable sticky notes.  
✔ **Minimize/Expand:** Clicking minimize hides/shows the note content.  
✔ **Close Sticky:** Clicking close removes the sticky note.  
✔ **(Not Yet Implemented)** Stickies are **not yet shared** across users in real time.  

---

## **📷 Image Handling**
✔ **Upload Images:** Users can upload an image and place it on the whiteboard.  
✔ **Download Board:** The entire board can be saved as an image (`.png`).  

---

## **🖥️ UI & User Interaction**
✔ **Hamburger Menu:** Toggles the toolbar visibility.  
✔ **Tool Selection:** Users can switch between **pencil, eraser, and sticky note**.  
✔ **Dynamic Resizing:** The board automatically adjusts to window size.  

---

## **🔄 Real-Time Collaboration with Socket.IO**
✔ **Live Drawing Sync:** Users see each other's drawings in real time.  
✔ **Sync Tool Changes:** If a user switches tools (pencil/eraser), others see the change.  
✔ **Sync Color & Size Changes:** Updates all connected users with the same brush settings.  
✔ **Undo/Redo Sync:** If a user undoes or redoes an action, it reflects for everyone.  
✔ **Sync Hamburger Menu:** When one user toggles the toolbar, it reflects on all screens.  

---

## **🔍 Possible Enhancements**
1️⃣ **Make Sticky Notes Collaborative** (sync across users).  
2️⃣ **Persist Data** (store drawings in localStorage or a database).  
3️⃣ **Improve Drawing Smoothness** (use Bezier curves for better strokes).  



## Demo
https://rahulsingh2003.github.io/White-board/
