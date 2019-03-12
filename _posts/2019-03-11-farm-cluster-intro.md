--- 
toc: true excerpt: "Getting you up and running R on
the UC Davis FARM computing cluster."
---

# Intro

This post is essentially a writeup of a \~2 hour in-person lesson I did
for a few friends who were interested in using the UC Davis CAES FARM
computing cluster. They both had a little experience, but not much,
working from the command line, and we were all on Macs, so it was pretty
easy to sit next to each other and have them follow along. Both of them
had similar needs as well: getting some long-running R scripts onto the
FARM to free up their computers, and maybe get some performance boosts
along the way.

This is by no means a comprehensive lesson on high performance
computing, nor is it a comprehensive lesson on using the Unix shell, nor
is it a compr… You get the idea: I’m not claiming to know all that much
about anything. This lesson is intended to help a novice get their R
scripts running on the FARM, using whatever strategy or philosophy I’ve
figured out to get **my** R scripts running on the FARM.

## What Will Be Covered

  - a few commands in Unix shell
  - accessing the FARM with SSH
  - moving files back and forth between FARM and your computer
  - basic SLURM commands on the FARM
  - pairing an R script and a SLURM submission script
  - general format for saving R results/outputs
  - how to install R packages on the FARM

## What Won’t Be Covered

  - parallelization of code
      - this is pretty specific to your task
      - I’m not good enough to feel comfortable giving a general
        overview
  - anything on Windows
      - ¯\\*(ツ)*/¯
  - a comprehensive description of any single topic
      - I’m not building the base of a pyramid here, I’m building a
        rickety ladder that will hopefully get you where you need to go
      - you can make that ladder less rickety or use it to access more
        places by building up a better foundation in the topics I’m
        touching on
  - other clusters
      - I’ve only ever worked on one cluster
      - while some of this may be generalized to other computing
        clusters, be careful

# Unix Shell Basics

![](/assets/rmd-images/farm-cluster-intro/ls_1.gif)

# Generating an SSH Key

# Getting Your Account

# Set Up Known Host

# Logging On and Looking Around

# `rsync` Basics

# Making Directories and Files

# `.R` and `.sh` Paired Scripts

# `sinfo` and `squeue`

# Submitting Jobs with `sbatch`

# Checking `stout` and `sterror`

# `rsync` Results Back

# `srun` Interactive R Session

# Set Up Directory for R Packages

# Install R Packages to Directory

# Load Packages from Here
