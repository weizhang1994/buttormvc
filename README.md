custom a php framework and add app on it.
1. create structure:: 

        public*:: The front of application
            index.php
            css*
                style.css
            js*
                main.js
            img*
            .htaccess:: mode_rewrite: could let us rewrite urls. if you type something in url couln't find, then this will  rewrite the url and then go back the index.php. 
        
        app*:: the entire mvc structure, library...
          libraries*::the heart of app
              core.php :: looking urls, pulling out what need to be pulled out
              database.php ::pdo class, include couple methods to select, update database. The Model will use this file
              controller.php ::we can easilly load models and views from other controllers
           models*
           views*
                pages* :: whatever we created in controller should have a view 
                        index.php
                        about.php
           controllers*
                Pages.php
           helpers*::for small things. like redirect helper, session helper
           config* :: the database, parameters..
           bootstrap.php :: basiclly it's gonna require all the files we need
           .htaccess:: we just don't want our app folder to be shown in phpmyadmin
           
         .htaccess:: we don't want our public dir show on phpmyadmin. we rewrite public to out root url
           
