# Directionality and Other features

Analyzer class and methods useful for directionality and general analysis on CYGNO reconstructed tracks.

First commit from commit `5d50321` of https://github.com/fiorotto8/CygnoAnal/tree/main 

## To compile

```g++ Analyzer.cxx Base_script.cxx -o nameprog `root-config --libs --cflags` -lSpectrum```

Optimized:
```g++ Analyzer.cxx Base_script.cxx -O3 -o nameprog `root-config --libs --cflags` -lSpectrum```

## To run

```./nameprog path_to_rootfile [output_directory]```

## Notes

- Rebinning is deactivated everywhere
- For MANGO He/CF4 fusion
  - ApplyThr(10)
  - RemoveNoise(30)
  - NPIP=250
  - wFac=2.
  - For 17keV PileUpCandidate(false, counter, true, 0.2, 2.0)
