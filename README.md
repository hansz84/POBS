POBS
====

POBS is a PHP Obfuscator. This means it "compiles" your PHP files by making them unreadable to a human.   

POBS - Installation
-------------------

Installing POBS is as easy as I could think of. Just unzip the downloaded file and put it a directory that is located under your web server. POBS is a collection of files in just 1 directory.

Before executing POBS you are advised to read the manual that is provided in the `doc` folder. Also check the settings in `pobs-ini.inc` and adjust them to suit your needs. When you run POBS for the first time you should at least adjust the `$SourceDir` and the `$TargetDir` variables.

If you have a large amount of PHP source to be POBSed, check your `php.ini` and see whether it runs in "Safe mode" (also, POBS warns for it). If it does, POBS can not adjust the timeout setting as indicated in `pobs-ini.inc` and the processing might be terminated before POBS has finished the replacement of all your PHP code files. You might need to restart your web server after adjusting the `php.ini` file.

After having checked everything and having adjusted the settings in `pobs-ini.inc` you point your browser to `pobs.php` and press `<Enter>`. 
