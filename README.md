# extract-specific-text-from-image

Using this script 'img_to_text.ipynb' -

You can extract emails from a screenshot. You can also extract other text based on your requirements and conditions.

Required libraries:

1. Pandas
2. Opencv
3. easyocr
4. os

I have added comments for every step in the script.

You might run into an error while trying to read images name from a folder.
Then you have take your images from the folder to the path where script is. Then you can use directory = os.listdir() without any argument.
But then, you have to specify the index range which your images belong to. You can run this for example directory = directory[4:8].
And then you in the loop you can run this to read every image reader.readtext(f'{directory}').
But you have to make sure that images are in such a sequence that they are all together or you can simply use try and except to pass it when there is an error which is
what will come up while trying to scan non-images.
