# HTML Music Player

This is a HTML music player that combines HTML and JQuery to give you a light weight music player which you can use from your desktop.

## Navigating and using the HTML Player

### How To Navigate To Your Favourite Artist Music Page

1. From the homepage click on the image of your favourite artist as seen in the image below.

![alt tag](https://s20.postimg.org/xdav4m8n1/_1.png)

2. Weldone, you've navigated to your favourite artist music page.

![alt tag](https://s20.postimg.org/iim9qfz25/_2.png)

### How To Play Music

1. Simply click on the song you want to play

![alt tag](https://s20.postimg.org/jyxs8l1z1/_3.png)

### How To Play The Next And Previous Song

1. To play the next song simply click on the double right arrow as shown in the image below.

![alt tag](https://s20.postimg.org/6w25pbbr1/_4.png)

2. To play the previous song simply click on the double left arrow as shown in the image below.

![alt tag](https://s20.postimg.org/n8c7f1q2l/_5.png)

## Modifying The HTML Music Player To Play Your Own Songs

1. Download A cover photo for the artist you want to add and save it in /Images.

2. Download/copy the music you want to play and paste them in /Music/YourArtist

3. Find Home.html and edit it in your favourite text editor/IDE.

4. Insert the following code under <div class=row>

	[comment]: <> (<div id="ImagePlaceHolder" class="col-sm-6">
		<a href="./YourArtist.html"><img class="img-thumbnail" src="./Images/YourArtist.jpg"></a>
		<p>Your Artist</p>
	</div>)

5. Create a new file named after the artist you're going to add e.g. yourartist.html

6. Copy all the code from BenHoward.html and paste it in yourartist.html

7. under <tbody> (line 32) replace the song details with the details of your artists song in the format seen below:

	[comment]: <> (<tr id="1" class="row-link">
		<td>Your Artist</td>
		<td>The Song</td>
		<td>The Album</td>
	</tr>)

8. Scroll down to line 162 and replace the image path to the path of your artists image, example shown below:

	[comment]: <> (var imagesrc1= './Images/YourArtistImage.jpg';)

9. Scroll down to line 165 (according to BenHoward.html) and replace the paths of the song and the name of the song with your artist songs path and song names as seen in the example below:

    [comment]: <> ({"song": path+'Your Artist Album/Song1.mp3', "name": "Your Artist - Song1"},
	{"song": path+'Your Artist Album/Song2.mp3', "name": "Your Artist - Song2"},)

10. Scrool down to line 187 and replace the image.src of the songs if needed, example:

	[comment]:<> (image.src=imagesrc1;)
