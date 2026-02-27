**\[Program for Reading Triangle Information from STL Files -- Developed
in VS2022\]**

1\. Functionality

\- The program can read STL files.

> \* Filename example: SPL_ASCII.stl (see folder in the referenced image
> page)

- In the program, it can open any STL file (\*.stl).

\- The program can creates a class representing a triangle: CTri.

(CTri Class Details)

> \* Vertices coordinates: fv_xyz\[3\]\[3\] -- float type
>
> \* Triangle area: fv_area -- float type
>
> \* Both variables (fv_xyz, fv_area) are private.

\- Includes a member function to calculate the triangle area.

\- Can save triangle information to a file.

\* Output Filename: output.csv (saved in the same folder as the STL
file)

\* Total number of triangles: XXX

\* Average triangle area: (2 decimal places)

\* Minimum and maximum coordinates (X, Y, Z axes) -- each with 2 decimal
places:

\+ X-axis: min, max

\+ Y-axis: min, max

\+ Z-axis: min, max

![](C:\Users\BGM\Documents\media/media/image1.png){width="6.268055555555556in"
height="6.876388888888889in"}

→ Red box: displays the coordinates (XYZ) of the three vertices of each
triangle.

\-
![](C:\Users\BGM\Documents\media/media/image2.png){width="6.250793963254593in"
height="3.3734437882764654in"}Execution Result Window: Shows the
computed triangle data.

------------------------------------------------------------------------

**2. MFC Project Setup**

\- **Project name:** STL_TRI_GENERATE_MFC_BGM

\- **GUI Type:** Dialog

\- Implementation Steps:

> S1. Handle file reading and writing in code.
>
> S2. Enable file selection through the GUI.

The saved file should be generated in the same folder as the STL file.

(Support both console mode and MFC GUI mode simultaneously.)

\*Example -- 3D STL file of a simple hexagon:

![](C:\Users\BGM\Documents\media/media/image3.png){width="3.248611111111111in"
height="2.7354166666666666in"}![](C:\Users\BGM\Documents\media/media/image4.png){width="5.502083333333333in"
height="3.0055555555555555in"}\* Program GUI Layout**:**

> S3. **File Selection:**

- Button to select the STL file

- Selected file **full path displayed in a read-only text editor**

> S4. **Tri Calculation RUN!**

- Button to read the STL file and generate the required triangle
  information

> S5. **Exit:**

- Button to terminate the program
