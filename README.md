PHP-ProgressBar
===============

PHP command line progress bar that adapts to screen width and shows current ETA.


Currently tested only on few Linux distributions and OS X. Will probably not work on Windows devices, because calculating console window width differ. Contributions welcome.


**USAGE**
---------

Initialize `progressBar` before loop:

    $progressBar = new ProgressBar(250);


While in loop, use below code to display current progress:

    foreach($items as $i){
            
        echo $progressBar->drawCurrentProgress();

        // actual loop code here
    }

You can advance progress to certain step calling:
        
    echo $progressBar->drawCurrentProgress(150); //will display progress as 150 of 250 iterations


Feel free to change anything and send pull requests!

Happy coding.
