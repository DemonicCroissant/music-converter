# music-converter
A bash script for automatically converting music and sorting it into
directories based on the name of the artist.

How to use this script:
1) (One-time) Change the directory names and output filetype and format in the
   script to your liking and install `ffmpeg` if you don't have it.
   
2) cd to the directory where the input files are. Supported input filetypes
   and formats are everything that your build of ffmpeg can understand, which
   is typically all audio and multimedia formats you'll commonly come across.
   
3) (Only necessary with `--sort` or `-s`) Rename all files in the directory
   to fit the pattern of `<Artist> - <Title>.*`.
   
4) Run the script. Specify `--sort` or `-s` if you want the converted files
   to be sorted into directories based on the name of the artist. If not, the
   converted files will be in the directory specified by `$out`. Either way
   the original files will be moved to `$original`. 
