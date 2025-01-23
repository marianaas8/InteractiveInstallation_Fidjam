# Fidjam: Interactive Music Mixer with TUIO and Minim

**Fidjam** is an immersive and participatory interactive music mixer that blends **music**, **technology**, and **creativity**. This installation provides an intuitive and engaging way for participants to explore and interact with music using physical cubes and an interactive surface, leveraging the **reacTIVision framework** to track fiducial markers on the cubes.

---

## **How It Works**

### **1. Physical Interaction**
- The installation features **five cubes**, each representing a different aspect of music composition:
  - **Genre Cube**:  
    One cube is used to select the genre, with three faces corresponding to:
    - **Pop**
    - **Hip-Hop**
    - **Rock**
    Users can place this cube in any position on the surface to choose the musical style they want to explore.

  - **Instrument Cubes**:  
    The other four cubes represent the instruments:  
    - **Drums**  
    - **Lead**  
    - **Vocals (Vox)**  
    - **Bass**  
    Each instrument cube has three faces, each representing a unique sound sample for that instrument. By positioning the cube with the desired face facing up, the corresponding sound sample is activated.

![cubes](https://github.com/user-attachments/assets/75a47c66-4ad6-46d3-bb53-e1b96f5f1825)


---

### **2. Interactive Surface Controls**
The interactive surface is used to control **volume** and **sound filtering**:
- **Volume Control**:  
  The vertical position (Y-axis) of the cubes adjusts the volume:
  - Higher positions = **louder sound**  
  - Lower positions = **quieter sound**  

- **Filter Control**:  
  The horizontal position (X-axis) of the cubes controls a **low-pass** and **high-pass filter**:
  - **Left** = Stronger **low-pass filter** (dampens higher frequencies).  
  - **Right** = Stronger **high-pass filter** (dampens lower frequencies).  

Through these intuitive physical interactions, users can adjust the **volume** and apply **dynamic filters** in real time, creating an immersive and hands-on experience for shaping music.

![surface](https://github.com/user-attachments/assets/2df88447-04d3-4ca9-be3f-2aa9a21d212a)

---

## **Setup Instructions**

### **1. Print the Interactive Surface and Cubes**
   - **Interactive Surface**: Print the `surface.pdf` file, preferably in **A3** format for better scaling and visibility.
   - **Cubes**: Print the `cubes.pdf` file to create your own DIY cubes. Make sure to associate the fiducial markers correctly with each cube face. Below are the markers for each genre and instrument:
   
     - **Genre Cube**:
       - **Face 1**: Pop - Marker ID: `11`
       - **Face 2**: Hip-Hop - Marker ID: `6`
       - **Face 3**: Rock - Marker ID: `12`
   
     - **Instrument Cubes**: Each instrument cube has three faces, representing different sound samples. These faces are associated with different marker IDs for each instrument:
       - **Drums Cube**:
         - Face 1: Marker ID `14`
         - Face 2: Marker ID `16`
         - Face 3: Marker ID `22`
       - **Lead Cube**:
         - Face 1: Marker ID `19`
         - Face 2: Marker ID `13`
         - Face 3: Marker ID `1`
       - **Vox Cube**:
         - Face 1: Marker ID `23`
         - Face 2: Marker ID `20`
         - Face 3: Marker ID `15`
       - **Bass Cube**:
         - Face 1: Marker ID `0`
         - Face 2: Marker ID `21`
         - Face 3: Marker ID `18`

### **2. Camera Setup**
   - Position the **camera** directly above the printed **interactive surface**. Make sure the entire surface is visible in the camera’s field of view.
   - The camera should be stable and not moved during interaction with the cubes to ensure accurate tracking.

### **3. Download Fidjam**
   - Download the `Fidjam.zip` file and unzip it.

### **4. Install Required Software**
   - [Download Processing](https://processing.org/download) and install it.
   - Install the following Processing libraries:
     - **Minim** (via the Library Manager).
     - **TuioProcessing** (from [TUIO.org](http://prdownloads.sourceforge.net/reactivision/TUIO11_Processing-1.1.5.zip?download)).
   - [Download Reactivision](http://prdownloads.sourceforge.net/reactivision/reacTIVision-1.5.1-win64.zip?download) for marker tracking.

### **5. Start Reactivision**
   - Open the Reactivision app and leave it open.
   - **Make sure Reactivision is using the correct camera feed** for marker tracking. The camera connected to your computer must be selected as the video input in the Reactivision settings.
   - Ensure that Reactivision is properly detecting the markers on the interactive surface.

### **6. Run Fidjam**
   - Open the `Fidjam.pde` file in Processing.
   - Press the **Run** button (play icon) to start the sketch.
   - Once the sketch is running:
      - Place the **Genre Cube** and **Instrument Cubes** on the interactive surface. 
      - Move the cubes vertically to control volume and horizontally to adjust filters.
      - Enjoy creating your personalized music mix in real time! 

