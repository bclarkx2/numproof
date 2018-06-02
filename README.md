
# numproof

This LaTeX package provides basic functionality for writing proofs. The format is based
off of the enumerate environment from the enumitem package. Each line is numbered, and 
the package provides several additional tools.

Please see the included .tex and .pdf files for an example.

<object data="numproof_test.pdf" type="application/pdf" width="700px" height="700px">
    <embed src="numproof_test.pdf">
    </embed>
</object>

## numproof environment

This is the outermost proof environment. The first argument dictates the title of the 
proof.


## subproof environment

This environment is the core of the package. The first argument sets the "proof depth". The numproof environment is essentially a subproof with depth=0. Use this environment to nest a subproof much like you would nest an enumerate environment inside another enumerate.


## Comments

You may insert a line comment onto the end of any numproof or subproof line using 
* \com to insert a simple, right justfied comment.
* \lines to insert a right justified line reference number. Can be used with a single line number or a range of line numbers (eg, 4-5)
* \comline to insert both a comment and a line number/range.

## Notes

The \note command will insert both a footnote at the bottom of the current page and 
a reference to the footnote at the end of the current line. Each additional footnote 
will use a different footnote symbol. The cycle of symbols resets when you make a new 
numproof environment.


## QED

The final line of a numproof will automatically include a QED box on the right of the 
page.


## Licensing

MIT (see LICENSE file)


## Authors

Brian Clark
