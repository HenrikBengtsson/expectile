# Version 0.3.1 [2015-11-11]

 * Package builds, installs and checks on modern R versions.
 
 * ROBUSTNESS: Properly import functions and declaring S3 methods.
 
 
# Version 0.3.0 [2012-06-22]

 * Now using `.onAttach()` instead of `.First.lib()`.
 
 * Now `sfit2()` passes NA instead of NULL to `.C("Rwrapper_sfit0")`.
 
 * BUG FIX: The previous workaround for using prior +Inf weights and
   pass them to the native code as .Machine$double.xmax did no longer
   work; it resulted in missing values in the results.  Passing Inf as
   `sqrt(.Machine$double.xmax)` seems to work.
   
 * Package passes R CMD check on R v2.15.0 and R devel.
 
 
# Version 0.2.6 [2012-03-23]

 * Now package uses `packageStartupMessage()` instead of `cat()` when
   loaded.
 
 
# Version 0.2.5 [2009-06-12]

 * Made `loexp()` internal for now.
 
 
# Version 0.2.4 [2008-12-26]

 * BUG FIX: Single-pass skewness calculation was incorrect. This could
   be the cause for poor convergence with some data sets.
 
 
# Version 0.2.3 [2008-09-08]

 * Updated the internal native sfit algorithm to fit the simplex/cone
   with a weighted prior simplex/cone.
 
 
# Version 0.2.2 [2008-08-31]

 * `fitCone()` calls `fitExpectileCone()` as is.
 
 * Added `fitExpectileCone()`, which returns an `ExpectileCone`
   object.
 
 * Added `points()`, `lines()`, and `radials()` to `ExpectileCone`.
 
 
# Version 0.2.1 [2008-08-03]

 * Added `loexp()`, which previously was in the **loexp** package.
 
 * Updated the help page for `sfit2()` and a fixed a bug in its
   examples.
 
 * Package passes `R CMD check` on R v2.7.1 and R v2.8.0 devel.
 
 
# Version 0.2.0 [2008-04-12]
 
 * Created.
