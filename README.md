Automatic File Sorting Program
Description
The Automatic File Sorting Program is a Python-based tool designed to help you organize files in a specified directory automatically. It sorts files into folders based on their file types (e.g., documents, images, videos, etc.). This tool can significantly streamline the process of managing files, especially in directories with a large number of files.

Features
Automatically sorts files into designated folders based on file types.
Customizable file type categories and destination folders.
Supports a wide range of file types (documents, images, videos, audio, etc.).
Easy to configure and use.
Requirements
Python 3.x
Libraries: os, shutil
Installation
Clone the Repository:

bash
Copy code
git clone https://github.com/yourusername/automatic-file-sorting-program.git
cd automatic-file-sorting-program
Install Required Libraries:

The program uses only built-in Python libraries, so no additional installations are required.

Usage
Configuration:

Edit the config.json file to customize the sorting rules. The default configuration is set to sort common file types:

json
Copy code
{
    "directories": {
        "documents": ["pdf", "doc", "docx", "txt"],
        "images": ["jpg", "jpeg", "png", "gif"],
        "videos": ["mp4", "mov", "avi"],
        "audio": ["mp3", "wav"],
        "archives": ["zip", "rar", "tar.gz"]
    }
}
You can add or modify the file extensions and their corresponding destination folders as needed.

Run the Program:

Execute the script with the target directory as an argument:

bash
Copy code
python file_sorter.py /path/to/your/directory
Replace /path/to/your/directory with the actual path of the directory you want to organize.

Example
Suppose you have a directory with the following files:

markdown
Copy code
/Downloads
    - report.pdf
    - image1.jpg
    - video.mp4
    - song.mp3
    - archive.zip
After running the program, your directory structure will be organized as follows:

bash
Copy code
/Downloads
    /documents
        - report.pdf
    /images
        - image1.jpg
    /videos
        - video.mp4
    /audio
        - song.mp3
    /archives
        - archive.zip
Contributing
If you would like to contribute to this project, please follow these steps:

Fork the repository.
Create a new branch (git checkout -b feature/your-feature).
Commit your changes (git commit -am 'Add new feature').
Push to the branch (git push origin feature/your-feature).
Create a new Pull Request.


Acknowledgements
Thank you for using the Automatic File Sorting Program. If you have any questions or feedback, please feel free to contact me at [your email address].
