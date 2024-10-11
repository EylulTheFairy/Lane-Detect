# Lane-Detect
My project for Teknofest Autonomous Taxi competition 2024.

I initially used Google Collab to write this code. You can reach that code here: https://colab.research.google.com/drive/1mVd6w7T0-bwkjXf7CXUuGbDKKIp2vwCp?usp=sharing

See this link for the road: https://drive.google.com/file/d/1v84yvYlFoX2NNgreq4MEvYnPJkxO_fZe/view?usp=sharing

File paths are of my own Google Drive. Relevant pickle files and video can be found in this repo or use your own material. You might have to make tweaks if you decide to use your own video.

## Some outputs:
Output of the road, grayscale with the polynomials on
![Output of the road , grayscale with the polynomials on](Output/1.png)
Output of the road, with trailing boxes and the polynomials
![Output of the road, with trailing boxes and the polynomials](Output/2.png)

## Notes:

1. You may want to tweak these two variables before running your video through the code as this will determine how your image will be "birdviewed". You will see a note at the very bottom of my code that might help you get good source-destination values without running the whole video through the code.
   ```
    source = np.float32([[1000,450],[1000, 720],[75,720],[200, 450]])
    destination = np.float32([[img_size[0], 0],
      [img_size[0]-offset, img_size[1]], [offset, img_size[1]],[0, 0]])
``
2. 
