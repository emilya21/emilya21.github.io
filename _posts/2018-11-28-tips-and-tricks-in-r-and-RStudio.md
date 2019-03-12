

(delete this)`--- toc: true excerpt: "A handful of useful things I've
picked up along the way." ---`(delete this)

I gave a (very informal) talk today for the [Davis R User’s
Group](https://d-rug.github.io/) where I shared some of my favorite
keyboard shortcuts, packages, and functions in R and RStudio. My basic
criteria for inclusion was anything that made me think “wow I wish I’d
learned this 6 months ago”. I keep a running list of these little tips
and tricks in a simple R script, and I polished it up (barely) for the
talk. Keeping with the low-effort nature of this whole thing, I’m just
going to post the script here in one big chunk, without much reordering
or reformatting. There’s not a ton of explanation about any of the tips
or tricks, so this should serve more to say “hey look at this thing that
exists” than “here’s a guide to this tool”. Hope you can find something
useful here\!

``` bash
cd ../../..
ls -a
```

    ## .
    ## ..
    ## .APKey.plist
    ## .CAS
    ## .CFUserTextEncoding
    ## .DS_Store
    ## .JGREditorprefsrc
    ## .JGRhistory
    ## .JGRprefsrc
    ## .MJ_Dns.txt
    ## .MJ_HD_Quality.txt
    ## .R
    ## .Rcache
    ## .Renviron
    ## .Rhistory
    ## .Rprofile
    ## .Trash
    ## .Xauthority
    ## .adobe
    ## .anaconda_backup
    ## .bash_history
    ## .bash_profile
    ## .bash_profile-anaconda.bak
    ## .bash_profile-anaconda3.bak
    ## .bash_profile-miniconda3.bak
    ## .bash_profile.macports-saved_2016-02-19_at_15:37:48
    ## .bashrc
    ## .bundle
    ## .cache
    ## .chemaxon
    ## .conda
    ## .config
    ## .credentials
    ## .cups
    ## .delta_configure
    ## .delta_configure.backup
    ## .dropbox
    ## .eclipse
    ## .emacs.d
    ## .emacs.d.bak
    ## .fontconfig
    ## .gem
    ## .gistr_code_file6921664b7f9e
    ## .gistr_code_filef1594be4fe20
    ## .gitconfig
    ## .gitkraken
    ## .iep
    ## .insert-shebang.log
    ## .ipython
    ## .jmf-resource
    ## .julia_history
    ## .jupyter
    ## .keras
    ## .lesshst
    ## .librc
    ## .local
    ## .matplotlib
    ## .netrc
    ## .npm
    ## .oracle_jre_usage
    ## .p2
    ## .pgadmin
    ## .pgadmin_histoqueries
    ## .pgpass
    ## .python_history
    ## .rnd
    ## .rstudio-desktop
    ## .spacemacs
    ## .spacemacs.env
    ## .spyder-py3
    ## .ssh
    ## .subversion
    ## .thumbnails
    ## .tooling
    ## .v8flags.6.0.286.52.f32d2c8c67d9a5d6c12cb68f25867a14.json
    ## .vim
    ## .viminfo
    ## .vimrc
    ## .wapi
    ## .wdc
    ## APH_Study_Protocol-blx.bib
    ## APH_Study_Protocol.aux
    ## APH_Study_Protocol.log
    ## APH_Study_Protocol.pdf
    ## APH_Study_Protocol.run.xml
    ## APH_Study_Protocol.synctex.gz
    ## APH_Study_Protocol.tex
    ## Adobe_Camera_Raw_Settings_Duplicate
    ## Adobe_Lightroom_Develop_Presets_duplicate
    ## AnacondaProjects
    ## Applications
    ## Bees-in-Space
    ## Bees-in-Space-20190228T172327Z-001.zip
    ## ColorBlindSafeTheme.css
    ## ColorBrewerCustomTheme.css
    ## Creative Cloud Files
    ## CytoscapeConfiguration
    ## Cytoscape_v3.4.0
    ## DRUG_talk_winter_18_final2.Rmd
    ## DRUG_talk_winter_18_final2.html
    ## DRUG_talk_winter_18_final2_cache
    ## DRUG_talk_winter_18_final2_files
    ## D_RUG_talk_winter_18.Rmd
    ## D_RUG_talk_winter_18_cache
    ## D_RUG_talk_winter_18_files
    ## D_RUG_talk_winter_18_final.Rmd
    ## D_RUG_talk_winter_18_final_cache
    ## D_RUG_talk_winter_18_final_files
    ## D_RUG_talk_winter_18_nonslide.Rmd
    ## D_RUG_talk_winter_18_nonslide_cache
    ## DataLab2Output
    ## Data_Class_Shiny_App
    ## Desktop
    ## Documents
    ## Downloads
    ## Dropbox
    ## ECL 232 Project Outline.aux
    ## ECL 232 Project Outline.log
    ## ECL 232 Project Outline.pdf
    ## ECL 232 Project Outline.synctex.gz
    ## ECL 232 Project Outline.tex
    ## ECL233Assignment8.png
    ## FARM_Fish_Models_1_24_19_clean
    ## Fish_Models_1_19_backup
    ## GitHub
    ## HD_log.txt
    ## LR_Presets_Mine
    ## LaTeX Files
    ## Library
    ## Making_My_Package.R
    ## Messed Up link Plot.png
    ## Movies
    ## Music
    ## NetLogo 5.2
    ## Nice non-link Plot.png
    ## Photographs
    ## Pictures
    ## PostgreSQL
    ## Projects
    ## Public
    ## PycharmProjects
    ## R Studio Files
    ## R_Packages_3.3
    ## R_Packages_3.4
    ## R_Packages_3.5
    ## RosenMac.gif
    ## RosenMacChangeSearchRange.gif
    ## Rplot.png
    ## Rplot01.png
    ## Rprof.out
    ## SimUText
    ## Sites
    ## TA_Orientation_Step_3.tnotes
    ## TESTEST
    ## Zotero
    ## Zotero_Library.bib
    ## ace_theme_test_script.R
    ## ag_app_notes_1_28_19.md
    ## ag_app_notes_1_28_19.md.temp
    ## asedump.js
    ## assignment5.gif
    ## bin
    ## bin2
    ## bis2b_spring17_lupine_plot.jpg
    ## bis2b_spring17_midterm_plot.jpg
    ## cron.log
    ## custom_chaos_theme.css
    ## desktop_launch_ecrib_4_31.jar
    ## example_biblatex_issue-blx.log
    ## example_biblatex_issue.aux
    ## example_biblatex_issue.bcf
    ## example_biblatex_issue.dvi
    ## example_biblatex_issue.log
    ## example_biblatex_issue.run.xml
    ## figure
    ## files
    ## git
    ## grad_tax_workshop.tnotes
    ## growth3.gif
    ## gulpfile.js
    ## img
    ## inclass.gif
    ## instagram-scraper.log
    ## java_launcher.prop
    ## league_rc5_annotated.tiff
    ## libs
    ## logo.gif
    ## meeting_with_Jay_2_6_18.tnotes
    ## miniconda3
    ## minimal_ggplot_theme.R
    ## node_modules
    ## old ipod movies
    ## package-lock.json
    ## packageNames.csv
    ## particles.gif
    ## pgadmin.log
    ## ri20min.rb
    ## rstudio-diagnostics
    ## scatterdeconstruct.gif
    ## stdlib
    ## test_farm
    ## test_farm_text
    ## test_file.csv
    ## test_file.feather
    ## test_profile.html
    ## test_script.py
    ## testtest.Rmd
    ## testtest.html
    ## testtest_after_hadley_ggplot2.Rmd
    ## testtest_after_hadley_ggplot2.html
    ## testtest_back_to_CRAN_ggplot2.Rmd
    ## testtest_back_to_CRAN_ggplot2.html
    ## testtest_backtodev_loadwithr.Rmd
    ## testtest_backtodev_loadwithr.html
    ## testtest_load_withr.Rmd
    ## testtest_load_withr.html
    ## texput.log
    ## tracktor-master
    ## vim_tutorial
    ## xaringan_test_slides.Rmd
    ## xaringan_test_slides.html
    ## xaringan_test_slides_files
