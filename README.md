custom a php framework and add app on it.
1. create structure
        public*::The front of application
            index.php
            css*
                style.css
            js*
                main.js
            img*   
        
        app*:: the entire mvc structure, library...
          libraries*::the heart of app
              core.php :: looking urls, pulling out what need to be pulled out
              database.php ::pdo class, include couple methods to select, update database. The Model will use this file
              controller.php ::we can easilly load models and views from other controllers
           models*
           views*
           controllers*
           helpers*::for small things. like redirect helper, session helper
           config* :: the database, parameters..
           bootstrap.php :: basiclly it's gonna require all the files we need
           .htaccess:: we just don't want our app folder to shown
           
