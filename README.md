# webcam config

Weblog post here: [How to webcam on Linux](http://reyhan.org/2013/09/webcam-on-linux.html)

## Get the config

```
cd ~/
git clone git@github.com:rey/.webcam.git
```

## Create symlinks

```
ln -s ~/.webcam/.webcamrc.1 ~/.webcamrc.1
ln -s ~/.webcam/.webcamrc.2 ~/.webcamrc.2
ln -s ~/.webcam/.screenrc.webcam ~/.screenrc.webcam
```

## Create handy bash alias

In your `.bashrc` add the following alias:

`alias watch='screen -S cam -c .screenrc.webcam'`

This creates a new screen session called `cam` using the `.screenrc.webcam` config.

## Start the session

`watch`
