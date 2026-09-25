Yes. Let’s define the setup precisely.

Suppose the two cases have the **same distance \(L\)** between the two points, but the object is elastically deformed differently along the travel axis:

* Case 1: deformation factor \(\lambda_1\), elastic potential energy \(U_1\), travel time \(t_1\)
* Case 2: deformation factor \(\lambda_2\), elastic potential energy \(U_2\), travel time \(t_2\)
* Same mass \(m\)
* Same travel distance \(L\)
* Total elastic + kinetic energy conserved.

The total energy is

$$
E=K+U=\frac12mv^2+U.
$$

Therefore,

$$
\frac12mv_1^2+U_1
=
\frac12mv_2^2+U_2.
$$

Rearrange:

$$
\frac12m(v_1^2-v_2^2)=U_2-U_1
$$

so

$$
v_2^2=v_1^2-\frac{2(U_2-U_1)}{m}.
$$

Since the distance is the **same**,

$$
t_1=\frac{L}{v_1},
\qquad
t_2=\frac{L}{v_2}.
$$

Hence

$$
\frac{t_2}{t_1}=\frac{v_1}{v_2}.
$$

Substitute \(v_2\):

$$
\boxed{
\frac{t_2}{t_1}
=
\frac{1}
{\sqrt{1-\frac{2(U_2-U_1)}{mv_1^2}}}
}
$$

and because

$$
K_1=\frac12mv_1^2,
$$

this becomes particularly clean:

$$
\boxed{
\frac{t_2}{t_1}
=
\frac{1}
{\sqrt{1-\frac{U_2-U_1}{K_1}}}
}
$$

### If \(U_2\gg U_1\)

Then approximately

$$
\boxed{
\frac{t_2}{t_1}
\approx
\frac{1}{\sqrt{1-\frac{U_2}{K_1}}}
}
$$

provided \(U_2<K_1\).

So as more of the conserved energy is transferred from kinetic energy into elastic energy, the velocity decreases and **the travel time increases nonlinearly**.

There is also an important limit:

$$
U_2\rightarrow K_1
$$

gives

$$
v_2\rightarrow0
$$

and therefore

$$
\boxed{t_2\rightarrow\infty}.
$$

If \(U_2>K_1\), the assumed motion cannot occur with those initial conditions—the system doesn't have enough kinetic energy to reach that deformation state.

### Bringing \(\lambda\) into it

If the elastic potential is approximately Hookean,

$$
U=\frac12 k(\Delta L)^2.
$$

If your deformation parameter \(\lambda\) means

$$
\Delta L=\lambda L,
$$

then

$$
U=\frac12k\lambda^2L^2.
$$

Therefore,

$$
U_2-U_1
=
\frac12kL^2(\lambda_2^2-\lambda_1^2).
$$

Putting this into the time relationship:

$$
\boxed{
\frac{t_2}{t_1}
=
\left[
1-
\frac{kL^2(\lambda_2^2-\lambda_1^2)}
{m v_1^2}
\right]^{-1/2}
}
$$

or, since \(K_1=\frac12mv_1^2\),

$$
\boxed{
\frac{t_2}{t_1}
=
\left[
1-
\frac{kL^2(\lambda_2^2-\lambda_1^2)}
{2K_1}
\right]^{-1/2}
}.
$$

**This is the relationship you're looking for if \(\lambda_1,\lambda_2\) represent the two elastic deformations.**

One caveat: if the object is being stretched **while the ball is actually moving**, rather than comparing two static deformation states, then \(U(x)\) changes continuously and \(t\) must be obtained from an integral \(t=\int dx/v(x)\). That gives a more interesting result than the simple endpoint-energy relation above.
