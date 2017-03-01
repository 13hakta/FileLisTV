## FileLisTV

FileLisTV is a TV to create file list on a Resource.
List can be output with TV render iterator.
Handy to create image sliders and file link set.

## How to Export

First, clone this repository somewhere on your development machine:

`git clone http://github.com/13hakta/FileLisTV.git ./`

Then, create the target directory where you want to create the file.

Then, navigate to the directory FileLisTV is now in, and do this:

`git archive HEAD | (cd /path/where/I/want/my/new/repo/ && tar -xvf -)`

(Windows users can just do git archive HEAD and extract the tar file to wherever
they want.)

Then you can git init or whatever in that directory, and your files will be located
there!

## Configuration

Now, you'll want to change references to FileLisTV in the files in your
new copied-from-FileLisTV repo to whatever name of your new Extra will be. Once
you've done that, you can create some System Settings:

- 'mynamespace.core_path' - Point to /path/to/my/extra/core/components/extra/
- 'mynamespace.assets_url' - /path/to/my/extra/assets/components/extra/

Then clear the cache. This will tell the Extra to look for the files located
in these directories, allowing you to develop outside of the MODx webroot!

## Information

Note that if you git archive from this repository, you may not need all of its
functionality. This Extra contains files and the setup to do the following:

- Integrates a custom table of "FileItem"
- A snippet listing Items sorted by name and templated with a chunk
- A custom manager page to manage FileItem on

If you do not require all of this functionality, simply remove it and change the
appropriate code.

Also, you'll want to change all the references of 'FileLisTV' to whatever the
name of your component is.

## Copyright Information

FileLisTV is distributed as GPL (as MODx Revolution is), but the copyright owner
(Vitaly Chekryzhev) grants all users of FileLisTV the ability to modify, distribute
and use FileLisTV in MODx development as they see fit, as long as attribution
is given somewhere in the distributed source of all derivative works.