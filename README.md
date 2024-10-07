Image to PDF Converter
This is a simple desktop application built using Tkinter and ReportLab that allows users to select multiple image files (PNG, JPG, JPEG) and convert them into a PDF. The application provides an easy-to-use graphical interface to select images, specify the output PDF file name, and save the images as a PDF file. A popup notification appears when the conversion is successful.

Features
Select multiple image files (supports .png, .jpg, .jpeg formats).
Preview selected images in a list.
Customize the output PDF file name.
Automatically adjusts image size to fit the PDF page while maintaining aspect ratio.
Displays a pop-up notification once the PDF is saved.
Requirements
The project uses Python's Tkinter library for the GUI and ReportLab to create the PDF. You will also need Pillow for handling images.

Dependencies
You can install the required dependencies using pip:

bash
Copy code
pip install pillow reportlab
How to Use
Clone the repository or download the script.

Install dependencies using the command mentioned above.

Run the application by executing the main function in the script:

bash
Copy code
python image_to_pdf_converter.py
Using the application:

Click the "Select Images" button to choose images from your file system.
The selected images will appear in a list.
Enter a desired PDF file name in the provided entry box (optional).
Click "Convert to PDF" to generate the PDF file.
A pop-up notification will confirm when the PDF has been saved successfully.
File Structure
image_to_pdf_converter.py: The main script that contains the ImageTOPDFConverter class and UI logic.
Code Walkthrough
ImageTOPDFConverter class: The main class that creates the GUI and handles image selection and PDF conversion.

select_images: Opens a file dialog for selecting images.
convert_images_to_pdf: Converts the selected images into a PDF file.
show_pdf_saved_popup: Displays a popup message when the PDF has been successfully saved.
Tkinter Listbox: Displays the selected image names.

ReportLab: Used to create the PDF document and insert images.

Pillow (PIL): Used to handle and manipulate image files.


