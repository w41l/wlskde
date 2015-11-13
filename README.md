WARNING
=======

STILL IN PROGRESS!

Please use AlienBOB KDE5 repositories below for complete Slackware Current KDE5 packages:
- http://alien.slackbook.org/ktown/ (the master repository),
- rsync URI: rsync://alien.slackbook.org/alien/ktown/
- http://taper.alienbase.nl/mirrors/alien-kde/ (my fast US mirror),
- rsync URI: rsync://taper.alienbase.nl/mirrors/alien-kde/
- http://repo.ukdw.ac.id/alien-kde/ (willysr’s Indonesian mirror),
- rsync URI: rsync://repo.ukdw.ac.id/alien-kde/
- http://slackware.org.uk/people/alien-kde/ (fast UK based mirror, run by Darren Austin),
- rsync URI: rsync://slackware.org.uk/people/alien-kde/

BUILDING
========

The building procedure is simple:

1. Clone this repository
```
  git clone https://github.com/w41l/wlskde.git
```

2. Change directory into wlskde and run:
```
  ./kde.SlackBuild
```

3. By default the build script WILL NOT upgrade already installed
   packages with same name. To "ALWAYS" install or upgrade the package,
   run the build script with environment variable:
```
  UPGRADE_PACKAGES="always" ./kde.SlackBuild
```

4. To install/upgrade single module (ie. just the 'plasma'), run:
```
  ./kde.SlackBuild plasma
```

5. To install/upgrade two or more modules, run:
```
  ./kde.SlackBuild frameworks,plasma
```

6. To install/upgrade single package or several packages, run:
```
  ./kde.SlackBuild plasma pkg1
  (or)
  cd plasma/pkg1 && ./pkg1.SlackBuild
  (or)
  ./kde.SlackBuild plasma pkg1:pkg2:pkg3
```

7. Use 'xwmconfig' to use KDE session for startx or start sddm at boot.

8. Reboot the machine is recommended.

THANKS
======

Thanks to AlienBOB for his complete KDE 5 SlackBuild: http://alien.slackbook.org/
