# Git-Docker Exam
This is a python application which gets images and creates a PDF file in a folder called “output” with all the images printed in it.

## build
    docker build -t convertor .

## runing
    docker run -it --rm --name my-running-convertor -v "$PWD/test/images":/usr/src/myapp/images -v "$PWD/test/output":/usr/src/myapp/output -e PDF_NAME=myenvironment convertor images
