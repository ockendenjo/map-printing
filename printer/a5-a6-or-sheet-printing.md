# A5/A6 or sheet printing

The manual paper feed on the printer should allow printing on any size paper smaller
than A4.

However, in practise the printer often seems to be confused about the orientation
of the paper and the document being printing and often cuts off edges.

I've found that the easiest way to print to A5 is to create an A4 PDF with multiple
copies of a course and then guillotine the paper after printing. 

The best way I've found to create a sheet is using the linux command line utility [pdfjam](https://github.com/rrthomas/pdfjam).

```shell
pdfjam yellow.pdf yellow.pdf --nup 2x1 --suffix 2up --landscape --outfile yellow-sheet.pdf
```

There may be free websites that can merge PDF pages in this way too
