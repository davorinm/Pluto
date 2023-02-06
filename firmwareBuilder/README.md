# Adalm Pluto Docker Firmware Builder


#### To build:

```bash
docker image build -t plutoFirmwareBuilder .
```

#### To run:

```bash
docker run -e DISPLAY=`hostname`:0 -it --rm -v $PWD:/home/phwl/work -w /home/phwl plutoFirmwareBuilder
```
