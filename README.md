# Transform Flow Data Sets

These data sets are designed to be used with the Transform Flow Visualisation tool. They are designed for sample usage, algorithm development, and testing/evaluation.

## Usage

Simply use the [transform-flow-visualisation][transform-flow-visualisation] command line tool, and point it to one of the data directories.

[transform-flow-visualisation]: https://github.com/HITLabNZ/transform-flow-visualisation

## Contributing

The data sets are deliberately compressed using 80% quality JPEG. The data capture tool captures high quality PNG files. To convert your files, use image magick:

	$ cd VideoStream-my-data-set
	$ mogrify -format jpg -quality 80% *.png
	$ rm *.png

You may wish to keep your PNG data sets, but in order to keep the repository size managable, we require JPEG only. Please use the exact conversion routine outlined above.

1. Fork it
2. Create your feature branch (`git checkout -b at-the-beach`)
3. Commit your data sets (`git commit -am 'At the beach'`)
4. Push to the branch (`git push origin at-the-beach`)
5. Create new Pull Request

## License

This work is licensed under a Creative Commons Attribution-ShareAlike 3.0 Unported License.

Copyright, 2013, by [Samuel G. D. Williams](http://www.codeotaku.com/samuel-williams).

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
