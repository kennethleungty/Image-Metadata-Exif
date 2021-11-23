# Read and Modify Image Metadata Extraction in Python with exif

Link to Medium article: https://towardsdatascience.com/read-and-edit-image-metadata-with-python-f635398cd991

### Context
For every photo, there is more than meets the eye. The photos taken with digital cameras and smartphones contain rich metadata, which is additional information about the image beyond the visible pixels.

This metadata can be useful in numerous business cases. For instance, fraud detection systems for insurance claims analyze metadata of submitted photographs to check whether the pictures were taken before the accident (aka date of loss).

In this project, we explore how we can utilize the exif library to read and edit the metadata of digital images.

The exif library can be installed with `pip install exif`


### Files and Folders
- `/sample_images`: Set of sample digital photos (by author) for metadata extraction and modification
- `/data`: Folder where the consolidated metadata are saved as CSV files
- `Image_Metadata_Extraction_EXIF.ipynb`: Notebook showcasing the different image metadata processing techniques (e.g. create, read, update, delete) with the exif library
- `batch_process_metadata.py`: Python script to batch process metadata of a set of images
   - This can be done by running this command in the terminal: `python batch_process_metadata.py`
   - The default folder is set as `sample_images`. To define the folder of the images designated for processing, you can use the --f attribute (string) to indicate folder name
   - For example, `python batch_process_metadata.py --f 'images_to_process'`
   - Output (CSV file) will be automatically saved in `/data` folder

### References
- https://exif.readthedocs.io/en/latest/
