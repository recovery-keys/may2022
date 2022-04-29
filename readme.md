# Backup [30-apr-2022]
# Backup version - v4


### Before Adding Image files:

`Move the new files to a temp folder.`

> mkdir temp

`add all the new img files`

`compress the png files`

> for i in *; do pngquant --quality=65-80 "$i" --ext _min.png --strip ; done

`copy the output to min location`
> cp *_min*.* ..

`strip metadata`
> for i in *; do exiftool -all= $i ; done

`remove src files`
> rm *.*_original

### Random Numeric Key Generator:

> for i in {88..98}; do openssl rand -base64 32 > $i.key; done

### Backup locations:
https://bitbucket.org/teta2064/may2022/
https://github.com/recovery-keys/may2022
https://gitlab.com/recovery-keys/may2022

### Tools

- veracrypt
- storj
- duplicity
- aws
- bitwardan

![alt text](https://raw.githubusercontent.com/recovery-keys/may2022/may2022/30-may-2022_flow.drawio.png)