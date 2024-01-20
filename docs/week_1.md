# Weekly report 1

Here we go! This is the start of the algorithms & AI lab course.  
During the first week I familiarised myself with the Moodle & course pages and made sure I know what to do during the course. This is the first of 6 weekly reports, which will document me implementing some algorithm.

The language is quite open on this course, so I decided to stick with what I know best: TypeScript.  
Knowing the working environment and the language well will aid in implementing a quite complex algorithm, and will not slow me down with having to figure out the language's quirks and features. In addition, using a well-known language will allow me to easily implement necessary tooling around the project, if I wish to e.g. benchmark improvements to the algorithm.

I decided to go with an algorithm instead of some small-scale AI project, as I'm still taking a linear algebra course that will help with AI projects in the future. Implementing a seemingly basic algorithm, the wave function collapse algorithm, still has a lot of quirks that need to be figured out. Creating the data stuctures required to have a fully functioning WFC implementation by the end of 6 weeks sohuld also prove a challenge. There are lots of of avenues to continue improving on WFC functionality, if I end up having a working implementation before the end of six weeks. It should also be quite an impressive demo.

Mostly I've been thinking about tooling and sources for the project. WFC is quite novel, in the way that it has not been formally documented, but rather is a simplified simulation of a much more complicated phenomenom in quantum physics. Since sources are sparce and there is no formal mathematic description of the algorithm, I will have to clearly document the choices made and improvements done. For this, great tooling should be in place. Spending an hour or two setting up a GitHub Actions pipeline should allow for faster development down the line, and robust benchmarking charts along the way.

As for the second week, it should already show a baseline implementation with existing TypeScript data structures. It will be naive, and slow, and probably not implement backtracking; but it should be a good base to improve on.