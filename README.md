### Janky way to somewhat keep themesongs in case my apartment's power goes out again aaAAAAAAA.

- [ ] update songs in here, maybe push from raspberrypi when $themesong command is successful?

In the case you forget how to use docker volumes, here's the command:

```
sudo docker run -v $(pwd)/data/mp3s:/bot/data/mp3s -d --name=mrbeats zeewalnut/mrbeats
```

`-v HOST_DIR:CONTAINER_DIR` don't forget `/bot` and waste hours on wondering why the `data/mp3s/` is empy when you forgor that `/bot` is the root of the container's dir, not `/data`
