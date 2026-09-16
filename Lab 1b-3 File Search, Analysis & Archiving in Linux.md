# 1b-3 File Search, Analysis & Archiving in Linux

## Archive Extracted
First thing I did for this lab activity was extract the compressed Gutenberg archive using the command "bunzip2".
<img width="550" alt="Screenshot 2026-09-13 141837" src="https://github.com/user-attachments/assets/a52db4da-f8ad-4c85-ae78-f4d787f6d759" />

## File listing
I used the command "ls" to list all the files I extracted from the archive and view the details of those files. It contains Moby, Frankenstein, and Two cities text file.
<img width="550" alt="Screenshot 2026-09-13 142107" src="https://github.com/user-attachments/assets/9c94217d-e128-4215-9049-bea759a1c661" />

## File name Search
Now here, I used the command called "find" with "-name "*.txt" to search for all the files inside my Downloads folder in my file manager. This confirms the location and also the filenames of all .txt files.
<img width="600" alt="image" src="https://github.com/user-attachments/assets/eb6e8498-8ecc-4cb8-9949-e3258b5606b6" />

## Search for String
I used the keyword "the", this will look for the files with "the" word inside the folder and display it.
<img width="600" alt="image" src="https://github.com/user-attachments/assets/899ccce6-be7b-4952-9a17-0c2772a553b5" />

## Search with context
I tried searching for "Next day" using the command "grep -r -C 3", which is not inside all three files so the result would be nothing.
<p><img width="600" alt="Screenshot 2026-09-16 142046" src="https://github.com/user-attachments/assets/14ab25e4-ef0d-4257-9a33-c851ed0cc352" /></p>

## Search for Dates
Now here I searched for the files with their dates indicated and the files are arranged from the oldest to newest file.
<img width="600" alt="image" src="https://github.com/user-attachments/assets/aa32efa6-f02b-42f1-a547-d1fab08d0407" />

## Search by file size 
For the file size, since the folder only have four files inside and 255258 bytes is a big files size, it will show nothing again for the result because all four files only have a small file size.
<img width="600" alt="image" src="https://github.com/user-attachments/assets/0bed9f07-103a-4696-9a7c-249661b6721a" />

## Find largest files
Here I tried looking for the largest files and here are the top 4 in my downloads, and also the largest one is the one at the top.
<p><img width="600" alt="image" src="https://github.com/user-attachments/assets/70ad7141-ef6b-486e-bb88-449bd094c65d" /></p>

## Frequency Analysis
For the frequency analysis, I tried checking the most occurring words used in the file called Moby.txt but all of the words only have 1 for word count.
<p><img width="600" alt="image" src="https://github.com/user-attachments/assets/6babe98d-b96b-41ed-bd30-392aaa19638f" /></p>

# Reflection
For this lab activity, I learned a lot of new commands and this time its for file searching and analysis. The command that I feel like was helpful and also I used a lot was the "find" command, this command is basically what I used most for searching for file name, dates, and file size. In cybersecurity, we often look for archive files that might be useful, and leaning this commands like "grep" and "find" can really make the searching process much easier and convenient. The only limitation I encounter doing this lab was the folder itself, because the folder only contains for files which made the searching process much faster and the files inside. Overall this lab activity help me gain more knowledge in using Linux commands.

