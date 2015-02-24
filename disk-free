#!/usr/bin/env bash

################################
# Shows info about a specified mount point
#
# @param {String} disk: The mount point to check
################################

full=""
short=""
color=""
status=0

disk=${BLOCK_INSTANCE:-/}


FS="$(df -h $disk | sed -n '2 p')"
FS=($FS)


if [ ${FS[4]%?} -ge 90 ]; then
    color='#47a8e9'
    status=33
fi

full="${FS[4]}"
short="${FS[4]}"


echo $full
echo $short
echo $color
exit $status
