### Jsteg is a package for hiding data inside JPEG files with a technique known as steganography. This is accomplished by copying each bit of the data into the least-significant bits (LSB) of the image. The amount of data that can be hidden depends on the file size of the jpeg; it takes about 10-14 bytes of jpeg to store each byte of the hidden data.

### Instalation of jsteg

```
$ sudo wget -O /usr/bin/jsteg https://github.com/lukechampine/jsteg/releases/download/v0.1.0/jsteg-linux-amd64
$ sudo chmod +x /usr/bin/jsteg
$ sudo wget -O /usr/bin/slink https://github.com/lukechampine/jsteg/releases/download/v0.2.0/slink-linux-amd64
$ chmod +x /usr/bin/slink
```

Jsteg successfully installed

![image](https://github.com/RahulMMenon011/Steganography/assets/140642506/573efa4b-206c-4c10-8385-4bb644cc589c)

Download a image file of any format and store in your directory, here i am using a file `flower.jpg` and create a simple text file which contains the message to be embeded in the file

![image](https://github.com/RahulMMenon011/Steganography/assets/140642506/6304ca87-8aff-41a8-af10-4998f4d2ffec)

### Hiding the data

```
jsteg hide <in.jpg> <secret file name> <out.jpg>
```

where in.jpg is our original file, secret file name is the name of text file and out.jpg is name of modified image file

![image](https://github.com/RahulMMenon011/Steganography/assets/140642506/9d8bb332-2409-4893-a49e-2466ab562288)

now the message is embedded into the new jpg file called flower_embeded.jpg

### Revealing the data

![image](https://github.com/RahulMMenon011/Steganography/assets/140642506/67c92ee9-c9ee-4366-9fa3-329c95532349)

msg revealed succesfully

