# docker-xenial-kraken

To create the DRIZZLECHAIR (instructions here: http://frostyhacks.blogspot.com.es/2015/04/gsm-wtf-bbq.html):

    docker run -ti --device=/dev/sdc:/dev/xvdc --device=/dev/sdd:/dev/xvdd --cap-add=SYS_ADMIN pachulo/xenial-kraken

To execute kraken (tips from https://docs.docker.com/engine/reference/commandline/run/):

    docker run -ti --rm --device=/dev/disk/by-id/wwn-0x5000c50091dc385d-part2:/dev/xvdc2 -v /media/$USER/DRIZZLECHAIR/kraken/indexes/:/kraken/indexes/ pachulo/xenial-kraken
