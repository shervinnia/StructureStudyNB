# Math

- To-do
    - Fourier transforms
        - What is a wave?
        - Different ways of representing a wave
        - Waves in image processing (analog vs digital representations
        - Fourier analysis, series, transforms
    - Operations
        - Convolution vs multiplication, differences between real and fourier space
    - Complex plane
        - Raising a number to $i$ and the origin/importance of $e$
        - $\exp(x)$ vs $e^x$

# Fourier Transforms

## What is a wave?

<aside>
💡 Note: in this text, “wave” will be used as substitute for sine and/or cosine waves. There are, of course, many other types of waves that are very relevant in other contexts. In this context, sine and cosine waves are the only relevant ones.

</aside>

A sine or cosine wave is a wave that describes its respective sine or cosine function where, in the context of a right triangle:

$$
\sin(\alpha)=\frac{\textnormal{opposite}}{\textnormal{hypotenuse}} \\\space\\\textnormal{and}\\\space\\\cos(\alpha) = \frac{\textnormal{adjacent}}{\textnormal{hypotenuse}}
$$

You may be able to quickly see the problem in that, in a triangle, you can only have $\alpha$ approach $90^\circ$, but never reach it. So, how do these functions repeat past $90^\circ$?

![hkndagiw.bmp](Math%20028303266b9646289cda6f2347c61144/hkndagiw.bmp)

We can construct a circle with $r = 1$ where we happen to label certain angles from the horizontal (or the $(1,0)$ point) with the corresponding distance along the perimeter of the circle to that same point.

This is simple to verify, you can find that the circumference is $C = 2\pi r = 2 \pi *1 =2\pi$. So, $\frac{1}{4}$ of the way around a circle of $360^\circ$ is $90^\circ$. Dividing the circumference by $\frac{1}{4}$ yields $\frac{\pi}{2}$. You can verify this for any point on the circle.

This is what we call the ***Unit Circle.*** Which also beautifully displays the relationship between the sine and cosine functions, best displayed in an animation.

[[Source](https://www.reddit.com/r/manim/comments/hnxioz/line_following_a_unit_circle/)](Math%20028303266b9646289cda6f2347c61144/undefined_-_Imgur.mp4)

[Source](https://www.reddit.com/r/manim/comments/hnxioz/line_following_a_unit_circle/)

## Different ways of representing a wave

Sine and cosine waves can realistically come in all shapes, size, and representations. So, what is the most basic way to represent them, and what is the purpose of other forms of visualizing them?

![download-modified.png](Math%20028303266b9646289cda6f2347c61144/download-modified.png)

To answer the first question, the three key components to create any sine wave are the following:

- **Frequency (or wavelength), $f \space(\textnormal{or}\space \lambda)$**: Number of full oscillations (peak-to-peak) in a given unit of time, usually seconds. This is equally substituted with wavelength (distance from peak-to-peak) in the context of physics as they can be related by $f = \frac{v}{\lambda}$
- **Amplitude, $A$:** The peak deviation of the wave from zero, presuming the wave is centered around an axis. The distance from the maximum to the minimum of the wave is double its amplitude.
- **Phase, $\phi$:**  The apparent shift in time of the wave by an amount in radians. A negative value represents a delayed start, a positive value represents an early start.

With just those three pieces of information, along with the knowledge of whether the wave is a sine or a cosine wave (otherwise, the phase will be off by $90^\circ$) any wave can be constructed.

Now the important part of this information, and the second part of our question, what are the other visualizations and why are they useful?

Realistically, any way of representing those three numbers is a way to represent a wave. The way you’re probably used to is something like the “anatomy of a wave” picture above. This visualizes the wave over the dimension it oscillates in, usually distance or time.

Another way of representing a wave is as a point on a graph, but in the frequency domain. The below figure illustrates such a representation compared to the time domain.

![Untitled](Math%20028303266b9646289cda6f2347c61144/Untitled.gif)

On the left,
