# ZFS_Configuration 

## Summary

Collection of scripts used for deploying, managing, and configuring my ZFS Storage Pools.

## Scripts

| script                   | description                                                  |
| ------------------------ | ------------------------------------------------------------ |
| create_homelab_zvols.yml | Provision all of the required ZFS datasets and their subvolumes for my personal homelab. Uses Ansible and iterates over a vars.yml file containing several nested lists detailing my personal storage configuration. Change `state` to absent in the role itself for each of the tasks to delete all of the ZFS datasets and their subvolumes. |
| sanoid.conf              | Configuration file for Sanoid. Defines ZFS Snapshotting policies for datasets and volumes deployed by `create_homelab_zvols.yml`. |
