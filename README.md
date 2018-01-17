
This is github.com/cortesi/devd inside a docker image.

Default command for devd is to simply serve files found in `/static` on the container. 

Sample Usage

```bash
docker run -i -p=8000:8000 --rm --mount type=bind,source=`pwd`,target=/static tahurt/docker-devd
```

(optionally) for custom devd behavior, like proxying, specify your devd flags at the end of the line, but be aware this overwrites the default command described above.
