# music-tiler
Generate image from all album artwork in a folder.

# Index

  - [Example](#example)
  - [About](#about)
  - [Todo](#todo)
  - [Pseudocode](#pseudocode)
  - [Resources](#resources)

## Example
Will create such images as this:

![](https://60stoday.com/wp-content/uploads/2017/08/7n5hqja.gif)
*I do not own or claim to own any of the artwork in this image. All artwork is copyright their respective authors.*

## About
Given a folder, will either tile all of the images (with a certain extension?) in that folder ***or*** use the Python [mutagen](https://mutagen.readthedocs.io/en/latest/) library to extract all album covers from music files (with `.mp3`, `.m4a`, etc).

## Todo
Everything. Specifically:

* Actually write some code.
* Then:
  * Make unit tests
  * Travis CI
  * Docker container

### Pseudocode

    from mutagen import File
    # Pillow for image processing?
    
    working_directory = input("Working directory (relative path): ")
    # Ask whether to use images or music tags
    # if filetype == "image":
    #     # make list of all images in working_directory
    # elif filetype == "music":
    #     # make list of all music files in working_directory
    # else:
    #     # Error.
    
    # if filetype == "music":
    #    # for each image:
    #         # extract album artwork if it exists
    
    # Crop all images to some size

## Resources

  - [How do I read album artwork using python? - Stack Overflow](https://stackoverflow.com/a/6173176/4381663)
