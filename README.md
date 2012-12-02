Problem: No [SMRT map](http://www.smrt.com.sg/Trains/NetworkMap.aspx) that's in a sane small SVG file

* [PDF](http://www.smrt.com.sg/Portals/0/PDFs/Trains/Network_Map_100112.pdf) is 92K, but [PDFs are bad](http://dabase.com/blog/PDF-A_versus_HTML/)
* [Website is unusable from a mobile](http://www.smrt.com.sg/Trains/NetworkMap.aspx) is huge and complex

Goal: Create small Web-friendly SVG for navigating [SMRT trains](http://en.wikipedia.org/wiki/SMRT_Trains)

# Plan of action

1. Split map.svg into:
	cck-line.svg green-line.svg legend.svg purple-line.svg red-line.svg yellow-line.svg
2. Convert [complex paths](http://s.natalian.org/2012-12-02/1354431225_1366x768.png) to simpler SVG constructs. Lots of SVG points to text
3. Re-combine `split-lines/*.svg` back into map.svg

# Tips

* Use [inkscape](http://en.wikipedia.org/wiki/Inkscape), save to plain SVG. Optimise SVG seems broken.
* [Resize page to drawing](http://s.natalian.org/2012-12-02/1354414212_1366x768.png)
* F2 to select text paths, F1 then delete to review

Using Droid Sans 18 size. Bold for junctions.
