# awesome-structured-light
Collect and organize some great structured light works.

1. **SLMaster**
   A very impressive structured light library.

   The code is here: [code](https://github.com/Practice3DVision/SLMaster)
2. **libStereoMatch**
   A practical stereo matching library.

   The code is here: [code](https://github.com/Practice3DVision/libStereoMatch)
3. **Zhang, Q., et al. (2012). "3-D shape measurement based on complementary Gray-code light." Optics and Lasers in Engineering 50(4): 574-579.**
   
   A method of using complementary Gray codes with higher frequencies for phase unwrapping is described, which only requires an additional projection of a higher frequency Gray code to complete any wrapped phase unwrapping with no more than 1/3 cycle phase error.

   The code is here: [cpu_version](https://github.com/Practice3DVision/SLMaster/blob/master/src/algorithm/cpuStructuredLight/sinusCompleGraycodePattern.hpp) and [cuda_version](https://github.com/Practice3DVision/SLMaster/blob/master/src/algorithm/gpuStructuredLight/cudaSinusCompleGraycodePattern.hpp)
4. **Wu, Z., et al. (2019). "High-speed three-dimensional shape measurement based on shifting Gray-code light." Opt Express 27(16): 22631-22644.**
   In order to avoid phase separation errors, the Gray code is shifted to the left by half a cycle to form a misaligned Gray code, thus perfectly avoiding the problem of phase separation failure caused by the intersection of cycles.

   The code is here: [code](https://github.com/Practice3DVision/SLMaster/blob/master/src/algorithm/cpuStructuredLight/sinusShiftGraycodePattern.hpp)
5. **Wu, Z., et al. (2021). "Generalized phase unwrapping method that avoids jump errors for fringe projection profilometry." Opt Express 29(17): 27181-27192.**
	The author keenly perceives that the phase misalignment of the wrapped phase can be used to avoid phase unwrapping errors. In this article, the author mentions a more general inter partition phase unwrapping method that can be applied to any phase calculation method and period determination method, such as PSP and Gray code methods.

    The code is here: [code](https://github.com/Practice3DVision/SLMaster/blob/master/src/algorithm/cpuStructuredLight/interzoneSinusFourGrayscalePattern.hpp)
6. **He, X., et al. (2019). "Quaternary gray-code phase unwrapping for binary fringe projection profilometry." Optics and Lasers in Engineering 121: 358-368.**
   A very impressive job. Compared to the traditional 0-1 grayscale, phase unwrapping at the same frequency requires a total of $log_2n$ Gray codes. In order to reduce the number of patterns and improve reconstruction efficiency, the author proposes using a four grayscale Gray code pattern, which only requires $log_4n$ Gray code patterns. Taking 16 cycles as an example, the two grayscale method requires a total of 4 patterns, while the four grayscale method only requires 2 patterns.

   The code is here: [code](https://github.com/Practice3DVision/SLMaster/blob/master/src/algorithm/cpuStructuredLight/interzoneSinusFourGrayscalePattern.hpp)

	


	
