vs2015 project for essentia-2.1_beta3

only configure for compile x86

https://github.com/MTG/essentia

use essentia_algorithm_reg.py to generate algorithms/essentia_algorithms_reg.cpp

//////////////////////////////////////////////////////////////////////////

modify files with flags [vs2015 compile modify]:

essentia\config.h
essentia\roguevector.h
essentia\stringutil.h
essentia\utils\jsonconvert.cpp
algorithms\standard\constantq.cpp

export and link modify
essentia\essentia\algorithm.cpp
essentia\essentia\algorithm.h
essentia\essentia\algorithmfactory.h
essentia\essentia\algorithmfactory_impl.h
essentia\essentia\debugging.cpp
essentia\essentia\debugging.h
essentia\essentia\essentia.cpp
essentia\essentia\essentia.h
essentia\essentia\parameter.h
essentia\essentia\streaming\streamingalgorithm.cpp
essentia\essentia\streaming\streamingalgorithm.h
essentia\essentia\types.h

//////////////////////////////////////////////////////////////////////////

remove files:
3rdparty\kiss_fft130\tools\fftutil.c
3rdparty\kiss_fft130\tools\psdpng.c

// todo gaiatransform use https://github.com/MTG/gaia
// remove now
algorithms\highlevel\gaiatransform.h
algorithms\highlevel\gaiatransform.cpp

// ffta only use in OSX / IOS , fft by Accelerate
algorithms\standard\iffta.h
algorithms\standard\iffta.cpp
algorithms\standard\ffta.h
algorithms\standard\ffta.cpp

//////////////////////////////////////////////////////////////////////////