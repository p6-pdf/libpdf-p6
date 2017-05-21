# lib-pdf

[![Build Status](https://travis-ci.org/p6-pdf/libpdf-p6.svg?branch=master)](https://travis-ci.org/p6-pdf/libpdf-p6) [![codecov](https://codecov.io/gh/p6-pdf/libpdf-p6/branch/master/graph/badge.svg)](https://codecov.io/gh/p6-pdf/libpdf-p6)

 <a href="https://ci.appveyor.com/project/p6-pdf/libpdf-p6/branch/master"><img src="https://ci.appveyor.com/api/projects/status/github/p6-pdf/libpdf-p6?branch=master&passingText=Windows%20-%20OK&failingText=Windows%20-%20FAIL&pendingText=Windows%20-%20pending&svg=true"></a>
Low level native library of PDF support functions.

The main aim is to optionally boost performance in the PDF tool-chain including
PDF stream and filter functions and PDF::Content image processing and encoding functions.

So far covered are:

- the widely used PDF::IO::Util `pack` and `unpack` functions.
- the PDF::IO::Filter::Predictor decode and encode functions.
- base64 encoding

Some other areas under consideration:

- C equivalents for other PDF::IO::Filter encoding functions, including predictors, ASCII-Hex, ASCII-85 and run-length encoding

- Support for PDF::Content::Image, including color-channel separation and (de)multiplexing. GIF decompression de-interlacing.

- Serialization. e.g. writing of literal or hex-encoded byte strings

There's sure to be others.

** Experimental Only **, at this stage.

Currently giving some benefits on work in development on larger PDFs.

This module will not be deployed until there as been significant advancement on Rakudo/MoarVM JIT, and I've
had a chance to benchmark this.


