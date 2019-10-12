# nsphere

In 2 dimensions (N = 2), consider the unity square (1 x 1 size). In it, inscribe a circle. What is the ratio between the area of the circle and the area of the square?

TBD insert image

In 3 dimensions (N = 3), consider the unity cube (1 x 1 x 1). In it, inscribe a sphere. What is the ratio between the volume of the sphere and the volume of the cube?

What happens when N = 4? N = 5? Or when N is arbitrarily large?

Does the volume of the inscribed N-sphere, compared to the volume of the N-cube, change when N varies? Is there a trend?

Would the volume ratios tend to a fixed value? If so, what is that value? Is it zero, or some other number?

## Monte Carlo

A good approximation of the volume ratio for any value of N can be obtained with the Monte Carlo method.

Generate a large number of dots within the cube, with random locations. Let's say the total number of dots is D.

Out of these dots, some will be inside the sphere, others will be outside. Count all the dots that are inside the sphere - let's say their total number is Ds.

TBD insert image

If you generate a very large number of dots, and they are random enough, then the sphere / cube volume ration is approximated by:

```
ratio = Ds / D
```

It's an "experimental" method that does not rely on exact analytic solutions.

## Results

It turns out, as N increases, the volume ratio decreases. As the number of dimensions keeps getting larger, the sphere appears to "shrink" in volume, as compared to the cube, even though the sphere is always inscribed in the cube.

TBD insert image

The decrease is sharp. Around N = 16, the volume ratio is essentially zero already.

Seems like, as N increases, there is more space available in the corners of the cube. The volume outside the sphere, in the corners of the cube containing it, becomes larger and larger. In comparison, the sphere becomes more and more insignificant.

Makes sense when you think about it for a while, but it's quite surprising at first.
