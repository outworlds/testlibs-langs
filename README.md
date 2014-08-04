testlibs-langs
==============

The purpose of this repository, as with all testlibs repositories, is to conduct tests and provide code samples for a
variety of related code libraries. The goal is to provide four series of tests:
1 Reliability
** The goal here is to prove that if I call the same function several times with the same input, that you will get the
same result back again and again. This is very rarely disproven; but what we also do is take a performance measurement
so we can check the consistency, and in some cases the scaling, of the function's timing.
2 Thread Safety
** Now take step 1 and apply it across multiple threads. Sometimes weird things happen. We can also check to see if the
function improves, or at least maintains, performance when multi-threaded.
3 Stress Testing
** Now we want to see how performant the function is when slammed by large numbers of threads, whether within the same
process, or called from external processes, if appropriate.

The testlibs-langs repository targets three main libraries and their various base classes, without stepping on the toes
of other testlibs repositories (like collections). Those libraries are:
1 java.lang (and some java.util and more)
2 org.apache.commons.lang3
3 com.google
