Docker container for running [Folding@Home](http://folding.stanford.edu/)

### Usage
```bash
docker run -d -p7396:7396 ultrasaber/folding-at-home:latest \
    --user=dude --team=11675 --gpu=false --smp=true --power=full --passkey=whatever
```

The web console is available on port `7396`.
