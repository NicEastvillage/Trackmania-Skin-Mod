# Trackmania skin mod for F-Klubben

This repo contains the files that make up the Trackmania skin mod for F-Klubben at Aalborg University.

![Exampl01](https://imgur.com/8ZpFPqF.png)

## How to use

### Textures

DOWNLOAD: http://dl.dropboxusercontent.com/s/y9dbnpnogwejx8v/FKlubben.zip

1. Go to your Trackmania user data directory. Typically `C:\Users\Me\Documents\TrackMania`.
2. Create a directory `Skins/Stadium/Mod` if it does not exist.
3. Put the downloaded `FKlubben.zip` in that directory (see download link above).
4. Open Trackmania.
5. Go to Editor and create a new track using the advanced editor. A "Choose skin" dialog should appear after picking decorations (time of day). If not, cancel and try holding `ctrl` while clicking all the buttons.
6. Do NOT select the "FKlubben" skin in this dialog. Instead, click "select URL" and paste the URL from above. Click "ok" and "ok" again. (We only downloaded the zip to make the "select skin" option appear in the first place. Trackmania is weird)
7. Done!
8. Side note: You have to select the skin using the URL *every time* you make a map in order to make it auto-downloadable by others.

The ancient but detailed guide can be found [here](http://trackmaniarpg.blogspot.com/2009/08/how-to-add-auto-downloadable-mod-to.html).

### Sign Pack

DOWNLOAD: See releases

1. Go to your Trackmania user data directory. Typically `C:\Users\Me\Documents\TrackMania`.
2. Create a directory `Skins/Any/Advertisement/FKlub` if it does not exist.
3. Open the downloaded `FKlubbenSigns.zip` and put its content in the created directory (see releases for download).
4. Open Trackmania and create a new map. Reskin a sign and you should be able to select `FKlub/Logo` and more.

### Individual Signs

This is for one-of signs, e.g. sponsors.

1. Create an image (preferably 256x128). Many file types are supported (even Bik videos!)
2. Upload it to [imgur.com](https://imgur.com/).
3. Copy the direct link to the uploaded image. Should be something like `https://imgur.com/YmDSiPV`.
4. Edit that link to `http://imgur.com/YmDSiPV.jpg` (switch to `http` instead of `https` and add file extension. Note that Trackmania don't like `.png` but `.jpg` is okay, even if the original image was a `png`. Yes, trackmania is weird)
5. While in the editor, reskin a sign and click "select URL". Pasted the edited URL.
6. On subsequent placement of signs, it will use the latest used skin. You can also find you sign among the existing options, but it will be called `YmDSiPV` or whatever the image is called in the link.

## How to edit

### Textures

The original textures can be found in the game's installation directory. Typically `C:\Program Files (x86)\Steam\steamapps\common\TrackMania United\GameData\Stadium\Media\Texture\Image`. However, only some of the textures can be replaced. See examples of other texture mods and textures that can be edited [here](http://trackmaniarpg.blogspot.com/2009/07/mods.html).

The textures are stored as `dds` files (direct draw surface) which is a compressed image format used in game. The non-transparent images are compressed using BC1 (Linear, DTX 1) format, while transparent images are compressing using the BC3 (Linear, DTX 5) format (although, transparent textures does not seem to be replaceable by mods). Paint.NET can save as `dds` files and can open the `pdn` files of this repo.

During editing, note that you must restart Trackmania every time you change a texture in the skin's zip file. Otherwise you are not guaranteed to see your changes.

**Uploading:**

1. After you have edited the skin, zip the textures to a `FKlubben.zip`.
2. Upload the zip to somewhere, where you can get a direct download link. I used Dropbox, but beware of the following:
   1. If `https://www.dropbox.com/s/y9dbnpnogwejx8v/FKlubben.zip?dl=0` is your share link, then it must be edited to `http://dl.dropboxusercontent.com/s/y9dbnpnogwejx8v/FKlubben.zip` (switch to `http` instead of `https`, change host, and remove `?dl=0`)
3. Edit this README such that the download link is correct.

### Sign Pack

* Signs are preferably 256x128 in size. Many file types are supported (even Bik videos!), but 

* Signs must be uploaded to [imgur.com](https://imgur.com/) or an alternative image host.
* Your `MySign.png` must be companied by a `MySign.png.loc` file, which contains a link to the direct download link of the image and it must be http.
  * E.g. if you image is uploaded to imgur as `https://imgur.com/YmDSiPV`, then the loc file should contain the link `http://imgur.com/YmDSiPV.png` (Note, Trackmania does not like `png` files when using the "select URL" option in the editor, but `png`s from `loc` files are okay. Trackmania is weird)

After editing the sign pack of this repo, zip the signs as `FKlubbenSigns.zip` and make a new release.

An ancient but detailed guide on `loc` files can be found [here](https://steamcommunity.com/sharedfiles/filedetails/?id=147553218).