# Build ITAPS from scratch

The purpose of this Homebrew tap is to build the
[ITAPS](http://trac.mcs.anl.gov/projects/ITAPS/wiki) collection of
software packages for mesh management in physics simulations.

This endeavor requires custom Homebrew formulas for:

- [MOAB](https://bitbucket.org/fathomteam/moab)
- [OpenCascade Community Edition](https://github.com/tpaviot/oce) (OCE)
- [CGM](https://bitbucket.org/fathomteam/cgm)
- [Lasso](https://bitbucket.org/fathomteam/lasso)

so that [PyTAPS](https://bitbucket.org/fathomteam/pytaps) can be built
with (nearly) full functionality.

Time permitting, formulas for

- PyTAPS
- [MeshKit](https://bitbucket.org/fathomteam/meshkit)

will be added so that MeshKit Python bindings can be built.

A long-term goal will be to merge the formulas in this tap into
[homebrew/science](https://github.com/Homebrew/homebrew-science).

# Rationale

Formulas already exist in homebrew/science for MOAB and OpenCascade
Community Edition. CGM requires a patched version of OCE or the
official OpenCascade version (OCC). The required patches have not been
submitted upstream to OCE, which makes it more difficult to submit the
required changes in this tap to homebrew/science. I have contacted the
CGM developers to make them aware of this situation, and hope that the
patches can be merged into OCE.

# TODO:

- Add installation instructions
- Add MOAB formula.
- Add OCE formula.
- Add patches to OCE formula.
- Add CGM formula.
- Add Lasso formula.
- Add instructions for installing PyTAPS using pip.
