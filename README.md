# ThreeJS Googly Eyes

Instant Googly Eyes for ThreeJS! Enjoy!

# Examples:

- [Googly Eyes on Suzanne](https://derschmale.github.io/threejs-googly-eyes/example/index.html)

# Usage

GooglyEyes are made to simply create and add to an existing model. Moving/rotating the model will cause the googly eyes
to update correctly when calling the `update` method.

Add it to your project:
```
npm install @derschmale/threejs-googly-eyes
```

And add it to your code!

```
// ... (whatever ThreeJS code)

import GooglyEyes from "@derschmale/threejs-googly-eyes";

// metric units are generally assumed
const eyes = new GooglyEyes(0.03, 0.05);
eyes.position.z = 0.1;

someModelThatNeedsGooglyEyes.add(eyes);

// ...

// your game-loop:

eyes.update(1 / 60); // can also pass in a custom timestep using THREE's Clock.


```

# Building

```
npm install
npm run build
```

# Example

To launch the example

1. Ensure that dependencies and code built

1. Launch host server e.g.


```bash
npm install -g http-server
http-server
```

3. Launch the sample in your browser e.g. [https://localhost:8080/example](https://localhost:8080/example)

Notes:
1. The example will move head with mouse movement and shift key
