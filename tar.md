# tar

Extract contents of tarball into directory other the current one

    tar -xvfz stuff.tar.gz -C /other/path
    
Create tarball for directory `book`

    tar -czvf 'Lions, Tigers, and Bears.tar.gz' book
    
List all files in tarball

    tar -tvf book.tar.gz

Create tarball but rename all paths that start with book to my-book

    tar -czvf 'Cool Book.tar.gz' -s /^book/my-book/ book
