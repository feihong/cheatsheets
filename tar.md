# tar

Extract contents of tarball into directory other the current one

    tar -xvfz stuff.tar.gz -C /other/path
    
Create tarball for directory `book`

    tar -czvf 'Lions, Tigers, and Bears.tar.gz' book
    
List all files in tarball

    tar -tvf book.tar.gz
