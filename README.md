Docker container for running [Folding@Home](http://folding.stanford.edu/)

### Usage
```bash
docker run -d -p7396:7396 -p36330:36330 ultrasaber/folding-at-home:latest \
    --user=foo --team=0 --smp=true --power=full --passkey=whatever --password=passwordgoeshere
```

All FAHClient command line arguments (see `docker exec <container> FAHClient --help`) are supported, to my knowledge.

#### Web console
The web console is available on port `7396`

#### Remote control
The client will listen for remote commands on `36330`. Note that you will need to use the `password` provided in the arguments in order to connect.
