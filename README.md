# Instructions to run application

1.  Create a Python 3.10.15 environemnt of
2.  Install Ollama: https://ollama.com/download
3.  Install requirements in requirements.txt

```bash
pip install -r requirements3.txt
```

4. export the api keys into your terminal or setup an env file. (In whatsapp)


5. Run the file `server/app.py` (This is the latest)

```bash
python server/app.py
```

6. Navigate to http://127.0.0.1:5000/menu/1 to open the menu page.


# Description of what is happening in the `main4.py` file

1. The book as a PDF is converted to images

-   Book is the `data/Blossoms of Savannah.pdf`
-   Output is in `images_from_pdf`

2. The images are then converted to text

-   Output is in `text_from_images`

3. The text is then split into chunks and stored in a vector database

-   The vector database is the `chroma_db` folder

4. The terminal is set up in preparation for asking questions

# Things to note

-   One needs `Ollama`. Install from [here](https://ollama.com/download) based on your OS
-   One specifies the type of model for Ollama. I use a `llama3.2:1b` since it is small(1.3 GB)
