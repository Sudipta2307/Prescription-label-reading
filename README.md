The "Prescription Label Reading Using OCR and Text-to-Speech" project aims to assist elderly and visually impaired patients by providing an innovative solution that reads out the information on prescription labels. This project leverages Optical Character Recognition (OCR) and Text-to-Speech (TTS) technologies to achieve its objectives.

The primary goal is to make medication management easier and safer for those who struggle with reading printed text due to age or visual impairments. Prescription labels often contain crucial information such as medication names, dosages, and usage instructions, which are vital for the correct and safe administration of medications. Misreading or misunderstanding this information can lead to serious health risks.

The project involves several key components:

OCR Module Using PaddleOCR:
The OCR module is responsible for recognizing and extracting text from images of prescription labels. PaddleOCR is chosen for its high accuracy and efficiency in text recognition, making it suitable for handling complex and varying fonts and layouts found on prescription labels.

Text Extraction Using PyMuPDF and Pytesseract:
For PDFs containing prescription information, PyMuPDF is used to extract both text and images from the document. If the prescription information is embedded within images, Pytesseract performs OCR on these images to accurately extract the text. This dual approach ensures that all relevant information is captured, regardless of its format within the PDF.

Text-to-Speech Conversion Using gTTS:
Once the text is extracted, it is converted into speech using the gTTS (Google Text-to-Speech) API. This conversion produces an audio file that can be played back to the user, providing a clear and understandable reading of the prescription information. The gTTS API is selected for its ability to generate natural-sounding speech, enhancing the user experience.

The implementation is designed to be user-friendly and accessible. Users can upload their prescription labels in the form of images or PDFs through a simple interface, such as Gradio. The system then processes the uploaded file, extracts the necessary text, converts it into speech, and provides an audio output that users can listen to. This process significantly reduces the reliance on others for medication management and promotes independence among elderly and visually impaired patients.
