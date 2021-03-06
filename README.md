# mucalc - convenient command line calculator

This calculator is intended for command line users.

It evaluates mathematical expressions that are given as arguments, read from
an input stream, or typed interactively.

In interactive mode, it provides line editing with tab-completion and
persistent history using [GNU readline](https://www.gnu.org/software/readline).

The evaluation of expressions is handled by the
[muParser](http://muparser.beltoforion.de/) math parser library.

Available constants:

- `pi`, `e`
 
Available functions:

- `deg`, `rad`,
- `sin`, `asin`, `cos`, `acos`, `tan`, `atan`, `atan2`,
- `sinh`, `asinh`, `cosh`, `acosh`, `tanh`, `atanh`,
- `pow`, `exp`, `exp2`, `exp10`, `log`, `ln`, `log2`, `log10`, `sqrt`, `cbrt`,
- `abs`, `sign`, `fract`, `int`, `ceil`, `floor`, `round`, `rint`, `trunc`,
- `min`, `max`, `sum`, `avg`, `med`,
- `clamp`, `step`, `smoothstep`, `mix`,
- `random`, `srand48`, `drand48`

Available operators:

- `^`, `*`, `/`, `%`, `+`, `-`, `==`, `!=`, `<`, `>`, `<=`, `>=`, `||`, `&&`, `?:`

Other features:

- Support for variables without explicit declaration
- Support for multiple expressions on one line, separated by commas
- Tab-completion for functions, constants, and variables

Example:

  `> sin(pi/2)`

  `1`
  
  `> sin(rad(90))`
  
  `1`
  
  `> a = 2^3 + 2`
  
  `10`
  
  `> b = sqrt(49) * 2 + 6`
  
  `20`
  
  `> sin(2 * pi) + a * b / log10(a^(b/4)) + cos(rad(12*(a+b))) + sign(a)`
  
  `42`
