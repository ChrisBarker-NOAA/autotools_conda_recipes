# autotools_conda_recipes

conda recipes to build the gnu autotools -- handy if you need to rebuild a configure script in a conda build.

# Why??

For teh most part, "official" source tarballs should include a confugure script ready to go, so you can build with the standard:
   
    ./configure && make && make install

dance.

But sometimes you need to pull from a source control repo, and it's a not a common (or good) practice idea to put generated files in source control. To build these, you need to run gnu autotools to build the configure script. This requires the gnu autotools. Linux systems (and systems like homebrew) generally provide them, but if you want to be able to build conda pacakges on a more bare bones system, you need autotools -- these recipes let you build the packages.


