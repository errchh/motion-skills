### Install Motion package via npm

Source: https://motion.dev/docs/react

Shows the npm command to install the Motion animation library and the import statement to access Motion components from the 'motion/react' module.

```bash
npm install motion
```

```javascript
import { motion } from "motion/react"
```

--------------------------------

### Install Motion for React using npm

Source: https://motion.dev/docs/react-installation

This command demonstrates how to install the Motion animation library for React applications using the npm package manager. Ensure you have Node.js and npm installed on your system before running this command.

```bash
npm install motion
```

--------------------------------

### Install Motion for React using Yarn

Source: https://motion.dev/docs/react-installation

This command illustrates the installation of the Motion animation library for React applications via the Yarn package manager. Yarn is an alternative to npm for managing project dependencies.

```bash
yarn add motion
```

--------------------------------

### Install Motion for React using pnpm

Source: https://motion.dev/docs/react-installation

This command shows how to install the Motion animation library for React applications using the pnpm package manager. pnpm is known for its efficient disk space usage and faster installations.

```bash
pnpm add motion
```

--------------------------------

### Enter animation with initial and animate props

Source: https://motion.dev/docs/react

Shows how to define entry animations using the initial prop for starting values and animate prop for target values. When the component mounts, Motion automatically animates from initial to animate state.

```javascript
<motion.button initial={{ scale: 0 }} animate={{ scale: 1 }} />
```

--------------------------------

### Configure animation duration with transition prop

Source: https://motion.dev/docs/react

Demonstrates how to customize animation behavior by passing a transition object within the animate prop. This example scales an element to 2x its size over 2 seconds.

```javascript
<motion.div
  animate={{
    scale: 2,
    transition: { duration: 2 }
  }}
/>
```

--------------------------------

### Scroll-triggered Animation with whileInView

Source: https://motion.dev/docs/react

Trigger animations when an element enters or leaves the viewport using the whileInView prop. This example animates background color and opacity as the element becomes visible. The initial state defines the starting animation state before the element enters the viewport.

```jsx
<motion.div
  initial={{ backgroundColor: "rgb(0, 255, 0)", opacity: 0 }}
  whileInView={{ backgroundColor: "rgb(255, 0, 0)", opacity: 1 }}
/>
```

--------------------------------

### Import Motion and create basic animated button component

Source: https://motion.dev/docs/react

Demonstrates how to import the motion library from 'motion/react' and create a simple animated button component with opacity animation. This is the foundational pattern for using Motion in React applications.

```javascript
import { motion } from "motion/react"

function Component() {
  return <motion.button animate={{ opacity: 1 }} />
}
```

--------------------------------

### Motion 12.0 Gesture Callback Migration Example

Source: https://motion.dev/docs/upgrade-guide

Example demonstrating the migration pattern for gesture callbacks in Motion 12.0. Previously, developers had to extract the target element from event properties. Now the element is provided directly as the first argument, eliminating unpredictability from target and currentTarget properties.

```javascript
hover("button", (element, startEvent) => {
  animate(element, { opacity: 0 })
  
  return (endEvent) => {}
})
```

--------------------------------

### Add Motion for React via CDN using jsDelivr

Source: https://motion.dev/docs/react-installation

This HTML snippet demonstrates how to include Motion directly into a web page using a Content Delivery Network (CDN) like jsDelivr. It uses a script tag with `type="module"` to import Motion as an ES module.

```html
<script type="module">
  import motion from "https://cdn.jsdelivr.net/npm/motion@latest/react/+esm"
</script>
```

--------------------------------

### Install Motion.js (Full Library) on Squarespace

Source: https://motion.dev/docs/squarespace

This snippet demonstrates how to install the complete Motion.js library on a Squarespace site by adding a script tag to the 'Code Injection' footer. It imports the `animate` function directly from the CDN and includes a basic example of animating an `h1` element's opacity. Users should replace the version number with the latest available.

```html
<script type="module" defer>
    import { animate } from "https://cdn.jsdelivr.net/npm/motion@11.13.5/+esm"

    // Your animation code here
    animate("h1", { opacity: [0, 1] })
</script>
```

--------------------------------

### Install Motion Studio SDK via npm

Source: https://motion.dev/docs/studio-sdk

Install the motion-studio package from the private Motion registry using an authentication token. Requires Motion+ membership to generate a private token. The command installs version 4.1.1 with specified package and token parameters.

```bash
npm install "https://api.motion.dev/registry.tgz?package=motion-studio&version=4.1.1&token=YOUR_AUTH_TOKEN"
```

--------------------------------

### Add hover and tap gesture animations with event handlers

Source: https://motion.dev/docs/react

Shows how to use whileHover and whileTap props for gesture-based animations, along with onHoverStart event handler. Motion provides cross-device gesture recognition for tap, drag, and hover interactions.

```javascript
<motion.button
  whileHover={{ scale: 1.1 }}
  whileTap={{ scale: 0.95 }}
  onHoverStart={() => console.log('hover started!')}
/>
```

--------------------------------

### Install Motion+ Package via npm

Source: https://motion.dev/docs/react-typewriter

Instructions for installing the `motion-plus` package using npm. This installation method requires a private token, which is exclusive to Motion+ members, to access the premium components.

```bash
npm install "https://api.motion.dev/registry.tgz?package=motion-plus&version=2.8.0&token=YOUR_AUTH_TOKEN"
```

--------------------------------

### Use Motion in Next.js App Router with client directive

Source: https://motion.dev/docs/react-installation

When using Motion with the Next.js App Router, components that utilize Motion must be client components. This example shows how to declare a component as a client component using the `"use client"` directive and then use a Motion component.

```javascript
"use client"

import { motion } from "motion/react"

export default function MyComponent() {
  return <motion.div animate={{ scale: 1.5 }} />
}
```

--------------------------------

### Install motion-plus Package with npm

Source: https://motion.dev/docs/react-animate-number

Installation command for the motion-plus package using npm with private token authentication. Requires Motion+ membership to generate a valid authentication token.

```bash
npm install "https://api.motion.dev/registry.tgz?package=motion-plus&version=2.10.0&token=YOUR_AUTH_TOKEN"
```

--------------------------------

### Install motion-plus package with authentication token

Source: https://motion.dev/docs/cursor

Install the motion-plus package using npm with a private authentication token. This requires an active Motion+ membership to generate the token. The command installs version 2.0.2 from the Motion API registry.

```bash
npm install "https://api.motion.dev/registry.tgz?package=motion-plus&version=2.0.2&token=YOUR_AUTH_TOKEN"
```

--------------------------------

### Configure Motion Studio MCP to Unlock Motion+ Features

Source: https://motion.dev/docs/studio-install

This JSON configuration snippet extends the basic MCP setup to unlock Motion+ features. It includes a personal access token in the `env` section, allowing the MCP to authenticate and provide premium functionalities like the codex and curve visualization. Replace `<YOUR_TOKEN>` with your actual Motion+ access token.

```json
{
  "mcpServers": {
    "motion": {
      "command": "npx",
      "args": ["-y", "https://api.motion.dev/registry.tgz?package=motion-studio-mcp&version=latest"],
      "env": {
        "TOKEN": "<YOUR_TOKEN>"
      }
    }
  }
}
```

--------------------------------

### Configuring `spring` with `keyframes` in JavaScript

Source: https://motion.dev/docs/spring

This example demonstrates the essential `keyframes` option for the `spring` function. It specifies that `spring` requires two numerical keyframes to define the start and end values for the spring animation.

```javascript
spring({ keyframes: [0, 100] })
```

--------------------------------

### Create a Steps Easing Function with 'start' Step Change

Source: https://motion.dev/docs/easing-functions

This example demonstrates how to modify the `steps` easing function to have the discrete steps change at the beginning of each interval by passing the 'start' option. This alters the timing of the jumps compared to the default 'end' behavior.

```javascript
const easing = steps(4, "start")

easing(0.2) // 0.25
```

--------------------------------

### useAnimationFrame Complete Setup - Vue Script Setup

Source: https://motion.dev/docs/vue-use-animation-frame

Complete Vue 3 component using useAnimationFrame with script setup syntax. Demonstrates importing the composable from 'motion-v', creating a template reference, and applying continuous animations to a DOM element. The callback receives both time (total elapsed) and delta (time since last frame) parameters for flexible animation control.

```vue
<script setup>
import { useAnimationFrame } from 'motion-v'

const domRef = ref()

useAnimationFrame((time, delta) => {
  domRef.value.style.transform = `rotateY(${time}deg)`
})
</script>

<template>
  <div :ref="domRef" />
</template>
```

--------------------------------

### Create rotating list element with Motion

Source: https://motion.dev/docs/react

Basic example of using the motion component to animate an HTML element. The animate prop defines target values that Motion will smoothly transition to using its hybrid engine.

```javascript
<motion.ul animate={{ rotate: 360 }} />
```

--------------------------------

### Importing and initializing a Motion Value in JavaScript

Source: https://motion.dev/docs/motion-value

This code demonstrates the basic setup for using `motionValue`. It shows how to import the `motionValue` function from the 'motion' library and initialize a new Motion Value with an initial numerical state.

```javascript
import { motionValue } from "motion"

const x = motionValue(0)
```

--------------------------------

### Install Motion.js (Mini Version) for Squarespace

Source: https://motion.dev/docs/squarespace

This snippet illustrates how to install the lightweight 'mini' version of the Motion.js `animate` function on Squarespace, which is optimized for file size. By importing from the `/mini/` path on the CDN, it provides a very small footprint, ideal for improving SEO scores while still enabling basic animations. Replace the version number as needed.

```html
<script type="module" defer>
    import { animate } from "https://cdn.jsdelivr.net/npm/motion@11.13.5/mini/+esm"

    // Your animation code here
    animate("h1", { opacity: [0, 1] })
</script>
```

--------------------------------

### Install Motion+ ScrambleText Package with npm

Source: https://motion.dev/docs/react-scramble-text

Provides instructions for installing the `motion-plus` package, which includes the `ScrambleText` component, using `npm`. This package requires a private token, indicating it's exclusive to Motion+ members.

```bash
npm install "https://api.motion.dev/registry.tgz?package=motion-plus&version=2.6.1&token=YOUR_AUTH_TOKEN"
```

--------------------------------

### Creating a `spring` Generator in JavaScript

Source: https://motion.dev/docs/spring

This example illustrates how to initialize a `spring` generator by providing an array of two `keyframes`. The generator can then be used to sample the spring's state at different points in time.

```javascript
const generator = spring({ keyframes: [0, 100] })
```

--------------------------------

### Run MotionScore audit via CLI

Source: https://motion.dev/docs/motionscore

Execute a MotionScore audit from the terminal using npx. The CLI prints a summary report directly in the terminal and provides a sharable URL to the audit results. Paid accounts can use the CLI to block CI/CD pipelines against minimum performance scores.

```bash
npx motionscore <url>
```

--------------------------------

### EVENT /onAnimationStart

Source: https://motion.dev/docs/vue-motion-component

Callback triggered when any animation (except layout animations) starts. It's provided a single argument with the target or variant name of the started animation.

```APIDOC
## EVENT onAnimationStart\n\n### Description\nCallback triggered when any animation (except layout animations, see `onLayoutAnimationStart`) starts.\nIt's provided a single argument, with the target or variant name of the started animation.\n\n### Type\nEvent\n\n### Arguments\n- **animationName** (string | object) - The target or variant name of the started animation.\n\n### Usage Example\n```vue\n<motion.circle\n  :animate=\"{ r: 10 }\"\n  @animationStart=\"latest => console.log(latest.r)\"\n/>\n```\n
```

--------------------------------

### Install Motion+ Animation Performance Audit Skill via cURL

Source: https://motion.dev/docs/animation-performance-audit

This command installs the Motion+ Animation Performance Audit skill into all detected AI editors. It uses 'curl' to fetch an installation script from the Motion.dev API and pipes it to 'bash' for execution. Users must replace 'YOUR_TOKEN' with their actual authentication token to successfully install the skill.

```bash
curl -sL "http://api.motion.dev/registry/skills/motion-audit?token=YOUR_TOKEN" | bash
```

--------------------------------

### Install Framer Motion 3D for React Three Fiber

Source: https://motion.dev/docs/react-three-fiber

This command installs the necessary packages for integrating Framer Motion 3D with React Three Fiber. It includes specific versions for `three`, `@react-three/fiber`, and `framer-motion-3d` to ensure compatibility. Note that Motion for React Three Fiber is currently compatible only with React 18.

```bash
npm install three@0.137.0 @react-three/fiber@8.2.2 framer-motion-3d@11.2.0
```

--------------------------------

### SVG Path Animation with pathLength

Source: https://motion.dev/docs/react

Animate SVG elements including special values for path drawing effects. This example animates the pathLength property of an SVG circle from 0 to 1, creating a drawing animation effect. Motion supports full SVG animation capabilities.

```jsx
<motion.circle animate={{ pathLength: 1 }} />
```

--------------------------------

### Collapsible Layout Animation Example

Source: https://motion.dev/docs/vue-layout-animations

Complete example of a collapsible component using layout animation. Demonstrates toggling height with the `layout` prop and handling click events to trigger layout changes.

```vue
<script setup>
const open = ref(false)
</script>

<template>
  <motion.div
    layout
    :style="{ height: isOpen ? '100px' : '500px' }"
    @click="() => open=!open"
  />
</template>
```

--------------------------------

### Generate CSS linear() Easing Curve for Springs

Source: https://motion.dev/docs/studio

Motion Studio empowers AI editors to generate CSS linear() easing curves, enabling the creation of springs or other custom easing effects directly within your editor. This example demonstrates a generated CSS linear() function representing a bouncy spring, derived from Motion code.

```css
600ms linear(0, 0.0121 /* ... */)
```

--------------------------------

### Disable initial animation on component mount

Source: https://motion.dev/docs/react

Demonstrates how to prevent the automatic entry animation by setting initial to false. The component will render at the animate values without transitioning from an initial state.

```javascript
<motion.button initial={false} animate={{ scale: 1 }} />
```

--------------------------------

### Basic useInView Setup in Vue

Source: https://motion.dev/docs/vue-use-in-view

Import and initialize the useInView hook with a template ref to track element visibility. Returns a boolean ref that updates when the element enters or leaves the viewport.

```vue
<script setup>
import { useInView } from 'motion-v'

const domRef = ref()
const isInView = useInView(domRef)
</script>

<template>
  <div ref="domRef" />
</template>
```

--------------------------------

### Illustrate `useMotionTemplate` tagged template syntax (React)

Source: https://motion.dev/docs/react-use-motion-template

This example clarifies that `useMotionTemplate` is invoked using JavaScript's tagged template literal syntax, rather than as a traditional function call. It highlights the specific syntax required for its usage.

```javascript
useMotionValue``
```

--------------------------------

### Scroll-linked Animation with useScroll

Source: https://motion.dev/docs/react

Link animation values directly to scroll position using the useScroll hook and MotionValues. This example scales the X-axis based on scroll progress, creating a progress bar effect. The scrollYProgress value ranges from 0 to 1 as the user scrolls.

```jsx
const { scrollYProgress } = useScroll()

return <motion.div style={{ scaleX: scrollYProgress }} />
```

--------------------------------

### Optimize Motion import for Next.js App Router

Source: https://motion.dev/docs/react-installation

To reduce the JavaScript bundle size delivered to the client in Next.js App Router, you can import Motion using `motion/react-client`. This alternative import is optimized for client-side usage, ensuring only necessary code is included.

```javascript
import * as motion from "motion/react-client"

export default function MyComponent() {
  return <motion.div animate={{ scale: 1.5 }} />
}
```

--------------------------------

### Configure Motion Studio MCP for Basic AI Features

Source: https://motion.dev/docs/studio-install

This JSON configuration snippet adds the basic Motion Studio MCP (Motion Control Protocol) server to your editor's settings. It uses `npx` to fetch and run the latest `motion-studio-mcp` package from the Motion registry, enabling AI enhancements like AI context and CSS spring generation.

```json
{
  "mcpServers": {
    "motion": {
      "command": "npx",
      "args": ["-y", "https://api.motion.dev/registry.tgz?package=motion-studio-mcp&version=latest"]
    }
  }
}
```

--------------------------------

### Exit Animation with AnimatePresence

Source: https://motion.dev/docs/react

Animate elements as they are removed from the DOM by wrapping motion components with AnimatePresence. The exit prop defines the animation state when the component unmounts. This example fades out the element with opacity 0 when removed.

```jsx
<AnimatePresence>
  {show ? <motion.div key="box" exit={{ opacity: 0 }} /> : null}
</AnimatePresence>
```

--------------------------------

### Integrating useReducedMotion in Vue 3 script setup

Source: https://motion.dev/docs/vue-use-reduced-motion

Shows how to import and utilize the `useReducedMotion` hook within a Vue 3 component's `<script setup>` block. It illustrates how to define a computed property (`closedX`) that dynamically adjusts an animation value based on the `shouldReduceMotion` state, enabling adaptive UI.

```vue
import { useReducedMotion } from 'motion-v'

const props = defineProps({
  isOpen: Boolean
})

const shouldReduceMotion = useReducedMotion()
const closedX = computed(()=>shouldReduceMotion.value ? 0 : '-100%')
```

--------------------------------

### Apply Value-Specific Transitions in Motion (Vue/JavaScript)

Source: https://motion.dev/docs/vue-transitions

This example demonstrates how to apply different transition settings to individual animated properties, while also providing a default transition for all other properties. This allows for complex animations where each value can have its own easing, duration, or type, enhancing visual richness.

```vue
// Motion component
<motion.li
  :animate="{
    x: 0,
    opacity: 1,
    transition: {
      default: { type: 'spring' },
      opacity: { ease: 'linear' }
    }
  }"
/>
```

```javascript
// animate() function
animate("li", { x: 0, opacity: 1 }, {
  default: { type: "spring" },
  opacity: { ease: "linear" }
})
```

--------------------------------

### Layout Animation with layout Prop

Source: https://motion.dev/docs/react

Enable automatic layout animations that detect and smoothly animate size, position, and reorder changes using transforms. The layout prop applies Motion's layout animation engine which corrects for scale-distortion unlike basic FLIP implementations.

```jsx
<motion.div layout />
```

--------------------------------

### React: Detailed example of useTime and useTransform for continuous animation

Source: https://motion.dev/docs/react-use-time

This detailed example illustrates the composition of `useTime` and `useTransform` to create a continuous, looping animation. `useTime` provides a constantly updating motion value, which `useTransform` maps from a time range (0-4000ms) to a rotation range (0-360 degrees), with `clamp: false` allowing for infinite rotation.

```javascript
const time = useTime()
const rotate = useTransform(
  time,
  [0, 4000], // For every 4 seconds...
  [0, 360], // ...rotate 360deg
  { clamp: false }
)
```

--------------------------------

### Define and Use a Custom Cubic Bezier Easing Function

Source: https://motion.dev/docs/easing-functions

This example demonstrates how to import and use the `cubicBezier` function to create a highly customized easing curve. It shows how to define the curve with four control points and then apply it to a progress value to get an eased output.

```javascript
import { cubicBezier } from "motion"

const easing = cubicBezier(.35,.17,.3,.86)

const easedProgress = easing(0.5)
```

--------------------------------

### Creating Exit Animations with `useAnimate` and `usePresence` in React

Source: https://motion.dev/docs/react-use-animate

This example demonstrates how to build custom enter and exit animations for components using `useAnimate` in conjunction with `usePresence` from Framer Motion. It shows how to detect component presence and trigger distinct animations for entering and exiting states, ensuring `safeToRemove` is called after exit animations complete.

```javascript
import { useAnimate, usePresence } from "framer-motion"

function Component() {
  const [isPresent, safeToRemove] = usePresence()
  const [scope, animate] = useAnimate()
  
  useEffect(() => {
     if (isPresent) {
       const enterAnimation = async () => {
         await animate(scope.current, { opacity: 1 })
         await animate("li", { opacity: 1, x: 0 })
       }
       enterAnimation()

     } else {
       const exitAnimation = async () => {
         await animate("li", { opacity: 0, x: -100 })
         await animate(scope.current, { opacity: 0 })
         safeToRemove()
       }
       
       exitAnimation()
     }
  }, [isPresent])
  
  return (
    <ul ref={scope}>
      <li />
      <li />
      <li />
    </ul>
  )
}
```

```javascript
<AnimatePresence>
  {show ? <Component key="dialog" /> : null}
</AnimatePresence>
```

--------------------------------

### Basic useInView Hook Setup in React

Source: https://motion.dev/docs/react-use-in-view

Demonstrates the fundamental usage of useInView hook with a ref object. The hook returns a boolean indicating whether the referenced element is currently visible in the viewport. This is the simplest way to track element visibility.

```javascript
import { useInView } from "motion/react"
import { useRef } from "react"

function Component() {
  const ref = useRef(null)
  const isInView = useInView(ref)
  
  return <div ref={ref} />
}
```

--------------------------------

### Setup motion components with Radix using asChild prop

Source: https://motion.dev/docs/radix

Demonstrates how to pass a motion component as a child to Radix components using the asChild prop to enable animation capabilities. The motion component can then use all standard animation props like initial, animate, and layout.

```jsx
<Toast.Root asChild>
  <motion.div
    initial={{ opacity: 0 }}
    animate={{ opacity: 1 }}
    layout
  />
</Toast.Root>
```

--------------------------------

### Handle hover start with element and event data

Source: https://motion.dev/docs/hover

Access both the hovered element and the triggering PointerEvent in the hover start callback to get precise coordinates and event information.

```javascript
hover("div:nth-child(2)", (element, startEvent) => {
  console.log("Hover started on", element)
  console.log("At", startEvent.clientX, startEvent.clientY)
})
```

--------------------------------

### Configure Animation Delay Parameter

Source: https://motion.dev/docs/animate

Sets the delay before animation starts in seconds with a default value of 0. Negative delay values start the animation partway through its duration. For example, delay: -1 starts the animation 1 second into its timeline.

```javascript
animate(element, { filter: "blur(10px)" }, { delay: 0.3 })
```

--------------------------------

### Getting the velocity of a Motion Value in JavaScript

Source: https://motion.dev/docs/motion-value

This example demonstrates how to obtain the current velocity of a `motionValue` using the `.getVelocity()` method. Velocity is intelligently calculated for number-like values and unit types, providing insight into the speed of change.

```javascript
const velocity = x.getVelocity()
```

--------------------------------

### Stagger Child Animations from Different Positions

Source: https://motion.dev/docs/vue-transitions

The 'stagger' function's 'from' option controls the starting point for staggering delays. Use 'last' to stagger from the last child, 'center' for center-outward, or a specific numeric index. This example staggers delays from the last child backwards.

```javascript
const transition = {
  delayChildren: stagger(0.1, { from: "last" })
}
```

--------------------------------

### Non-linear Sampling of `spring` Generator in JavaScript

Source: https://motion.dev/docs/spring

This example highlights the flexibility of the `spring` generator, showing that it can be sampled at arbitrary, non-sequential time points. This allows for advanced control over retrieving spring values without strict time-ordering.

```javascript
generator.next(100)
generator.next(10)
```

--------------------------------

### Create a continuous animation loop with Motion `frame.update`

Source: https://motion.dev/docs/frame

This example demonstrates how to set up a function to run continuously on every animation frame during the `update` step by passing `true` as the second argument to `frame.update`. It also includes logic to stop the loop after a certain number of iterations using `cancelFrame`.

```javascript
let i = 0

function update() {
  i++

  // Stop after 100 frames
  if (i >= 100) cancelFrame(update)
}

frame.update(update, true)
```

--------------------------------

### Shared Element Animation with layoutId

Source: https://motion.dev/docs/react

Create shared element animations between completely different components by assigning the same layoutId. This enables smooth transitions when elements are replaced or repositioned in the DOM.

```jsx
<motion.div layoutId="underline" />
```

--------------------------------

### Apply a Predefined Transition Object in Motion (Vue/JavaScript)

Source: https://motion.dev/docs/vue-transitions

This example demonstrates how to apply a previously defined transition object to an animation. It shows usage with a Motion component's `:transition` prop in Vue and with the `animate()` function in JavaScript, providing a consistent animation across different contexts.

```vue
// Motion component
<motion.div
  :animate="{ x: 100 }"
  :transition="transition"
/>
```

```javascript
// animate() function
animate(".box", { x: 100 }, transition)
```

--------------------------------

### Migrate from framer-motion to motion package

Source: https://motion.dev/docs/react-upgrade-guide

Uninstall the framer-motion package and install the new motion package, then update imports to use motion/react. This is the primary upgrade step for Motion for React version 12.0.

```bash
npm uninstall framer-motion
npm install motion
```

```javascript
import { motion } from "motion/react"
```

--------------------------------

### Import Specific Easing Functions from Motion Library

Source: https://motion.dev/docs/easing-functions

This example shows how to import individual easing functions, such as `easeIn`, directly from the 'motion' library. This allows for standalone use of the easing functions, either for custom animations or integration with the tiny `animate` function from 'motion/dom'.

```javascript
import { easeIn } from "motion"
```

--------------------------------

### Handle Press Start Events

Source: https://motion.dev/docs/vue-motion-component

The onPressStart callback fires when a pointer begins pressing the component. Receives the triggering PointerEvent as an argument.

```vue
<motion.div @pressStart="(event) => console.log(event)" />
```

--------------------------------

### Schedule a callback for rendering with Motion `frame`

Source: https://motion.dev/docs/frame

This example demonstrates how to schedule a function to execute during the `render` step of Motion's animation loop. The provided callback will run once on the next available animation frame, typically for applying visual changes to the DOM.

```javascript
frame.render(() => element.style.transform = "translateX(0px)")
```

--------------------------------

### Subscribing to Motion Value changes in JavaScript

Source: https://motion.dev/docs/motion-value

This example shows how to attach a listener to a `motionValue`'s 'change' event. The provided callback function will be executed every time the value of `x` updates, receiving the `latest` value as an argument.

```javascript
x.on("change", latest => console.log(latest))
```

--------------------------------

### Start drag from custom element with pointer event

Source: https://motion.dev/docs/react-use-drag-controls

Initiate a drag session from a different element by calling the start method on drag controls with a pointer event. This enables dragging to be triggered from arbitrary UI elements like video scrubbers.

```javascript
<div onPointerDown={event => controls.start(event)} />
```

--------------------------------

### Configure Global Default Transitions with MotionConfig (Vue)

Source: https://motion.dev/docs/vue-transitions

This example demonstrates how to set a global default transition for a group of `motion` components using the `MotionConfig` component. Any `motion` component nested within `MotionConfig` will inherit these transition settings, providing a consistent animation style across an application section.

```vue
<MotionConfig :transition="{ duration: 0.4, ease: 'easeInOut' }">
  <App />
</MotionConfig>
```

--------------------------------

### Detect Animation Start Events

Source: https://motion.dev/docs/vue-motion-component

The onAnimationStart callback triggers when any animation begins (excluding layout animations). Receives the target or variant name of the started animation as an argument.

```vue
<motion.circle
  :animate="{ r: 10 }"
  @animationStart="latest => console.log(latest.r)"
/>
```

--------------------------------

### Set Animation Sequence Timing Relative to Previous Animation Start

Source: https://motion.dev/docs/animate

Uses the 'at' parameter with '<+' or '<-' prefix to start an animation relative to the start of the previous animation. Enables precise timing offsets from the beginning of prior animations.

```javascript
const sequence = [
  ["nav", { opacity: 1 }],
  
  // 0.5 seconds after the start animation (0.5 secs):
  ["nav", { x: 100 }, { at: "<0.5" }],
  
  // 0.2 seconds before the start of the previous animation (0.3 secs):
  ["nav li", { opacity: 1 }, { at: "<-0.2" }],
]
```

--------------------------------

### Manually creating and animating a Motion Value in JavaScript

Source: https://motion.dev/docs/motion-value

This example demonstrates how to manually create a `motionValue`, subscribe to its `change` event to log updates, and then animate it from its initial state to a new value using the `animate` function. This is useful for advanced control over animated properties.

```javascript
const x = motionValue(0)

x.on("change", latest => console.log(latest))

animate(x, 100)
```

--------------------------------

### Serialize TransitionState to URL Query String in Motion Studio

Source: https://motion.dev/docs/studio-sdk-state

This example shows how to use the `toShareQueryString` utility from 'motion-studio' to convert a `TransitionState` object into a URL query string. This function enables the creation of shareable links that encapsulate the current animation configuration.

```typescript
import { toShareQueryString } from "motion-studio"

const queryString = toShareQueryString(state)
// Output: "transition=%7B%22type%22%3A%22spring%22...%7D"
```

--------------------------------

### Setup LazyMotion with domAnimation features

Source: https://motion.dev/docs/react-reduce-bundle-size

Wrap your application with LazyMotion and specify feature packages to load manually. The `domAnimation` package provides animations, variants, exit animations, and tap/hover/focus gestures (+15kb). Features are bundled into the main JavaScript bundle with this synchronous approach.

```javascript
import { LazyMotion, domAnimation } from "motion/react"

// Load only the domAnimation package
function App({ children }) {
  return (
    <LazyMotion features={domAnimation}>
      {children}
    </LazyMotion>
  )
}
```

--------------------------------

### Handle Pan Start Events

Source: https://motion.dev/docs/vue-motion-component

The onPanStart callback fires when a pan gesture begins. Receives the triggering PointerEvent and info object containing delta, point, offset, and velocity properties.

```vue
<motion.div @panStart="(event, info) => console.log(info.delta.x)" />
```

--------------------------------

### Detect Animation Start with `onAnimationStart` Callback in Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `onAnimationStart` callback fires when any animation (excluding layout animations) begins. It receives the target or variant name of the started animation, allowing for actions to be taken at the animation's onset.

```javascript
<motion.circle
  animate={{ r: 10 }}
  onAnimationStart={latest => console.log(latest.r)}
/>
```

--------------------------------

### Create a perpetual rotation animation with useTime and useTransform

Source: https://motion.dev/docs/vue-use-time

These examples demonstrate how to use `useTime` to get a continuously updating motion value and `useTransform` to map that time value to a rotation. It creates a perpetual rotation animation, suitable for both Vue components and general JavaScript contexts. `useTime` provides the elapsed time, and `useTransform` converts it into a rotation angle over a specified duration, with `clamp: false` ensuring continuous looping.

```vue
<script setup>
const time = useTime()
const rotate = useTransform(time, [0, 4000], [0, 360], { clamp: false })
</script>

<template>
  <motion.div :style="{ rotate }" />
</template>
```

```javascript
const time = useTime()
const rotate = useTransform(
  time,
  [0, 4000], // For every 4 seconds...
  [0, 360], // ...rotate 360deg
  { clamp: false }
)
```

--------------------------------

### Importing `transform` from Motion (JavaScript)

Source: https://motion.dev/docs/transform

This example illustrates how to import the `transform` function from the Motion library into your JavaScript project. It also notes that React users have access to a `useTransform` hook for similar functionality with motion values.

```javascript
import { transform } from "motion"
```

--------------------------------

### Set Drag Constraints using `useDomRef` in Vue

Source: https://motion.dev/docs/vue-gestures

This example demonstrates how to dynamically set drag constraints using an HTML element reference. It utilizes `useDomRef` from `motion-v` to get a reference to a parent `motion.div` and then passes this ref to the draggable child's `dragConstraints` prop, confining the drag within the parent's bounds.

```html
<script setup>
  import { useDomRef } from "motion-v"
  const constraintsRef = useDomRef()
</script>
<template>
  <motion.div ref="constraintsRef">
      <motion.div drag :dragConstraints="constraintsRef" />
  </motion.div>
</template>
```

--------------------------------

### Configure LayoutCamera with React Three Fiber and Motion Props

Source: https://motion.dev/docs/react-three-fiber-layout-cameras

This example illustrates how to apply both standard React Three Fiber properties and Framer Motion animation properties to a `LayoutCamera` component. It shows setting `position` and `zoom` for camera configuration, alongside `animate` and `transition` for dynamic animation control. This allows for complex camera movements and effects within layout animations.

```javascript
<LayoutCamera
  position={[0, 0, 5]}
  zoom={20}
  animate={{ zoom: 100 }}
  transition={{ duration: 2 }}
/>
```

--------------------------------

### Handle Hover Start Events

Source: https://motion.dev/docs/vue-motion-component

The onHoverStart callback fires when a pointer begins hovering over the component. Receives the triggering PointerEvent as an argument for custom hover logic.

```vue
<motion.div @hoverStart="(event) => console.log(event)" />
```

--------------------------------

### Setting a Motion Value with a string value in JavaScript

Source: https://motion.dev/docs/motion-value

This example demonstrates using the `set` method to update a `motionValue` with a string value, such as a color. This directly changes the value and triggers any associated listeners.

```javascript
x.set("#f00")
```

--------------------------------

### AnimateNumber with Advanced Transition Settings in React

Source: https://motion.dev/docs/react-animate-number

Advanced example showing how to configure value-specific transition settings for different animation properties (layout, opacity, y) in AnimateNumber using Motion's transition options.

```jsx
<AnimateNumber transition={{
  layout: { duration: 0.3 },
  opacity: { ease: "linear" },
  y: { type: "spring", visualDuration: 0.4, bounce: 0.2 }
}}>
  {count}
</AnimateNumber>
```

--------------------------------

### Integrating MotionCanvas for Context-Aware 3D Animations in React

Source: https://motion.dev/docs/react-three-fiber-motion-canvas

This example demonstrates how to set up a React application using `MotionCanvas` from `framer-motion-3d`. It shows importing `MotionConfig` and `motion` from `motion/react` for general motion, and `MotionCanvas` and `motion as motion3d` from `framer-motion-3d` for 3D elements. The `App` component then wraps a `MotionCanvas` within a `motion.div` to animate both 2D and 3D elements while preserving animation context.

```jsx
import { MotionConfig, motion } from "motion/react"
import { MotionCanvas, motion as motion3d } from "framer-motion-3d"
```

```jsx
export function App() {
  return (
    <MotionConfig transition={{ type: "spring" }}>
      <motion.div animate={{ scale: 2 }}>
        <MotionCanvas>
          <motion3d.boxGeometry animate={{ x: 1 }} />
        </MotionCanvas>
      </motion.div>
    </MotionConfig>
  )
}
```

--------------------------------

### Set Animation Sequence Timing to Previous Animation Start

Source: https://motion.dev/docs/animate

Uses the 'at' parameter with '<' string value to start an animation at the same time as the previous segment. Enables parallel animations within a sequence without explicit timing calculations.

```javascript
const sequence = [
  ["nav", { x: 100 }, { duration: 1 }],
  
  // This will start at the same time as the x: 100 animation
  ["li", { opacity: 1 }, { at: "<" }],
]
```

--------------------------------

### Handle Pan Start Event with `onPanStart` Callback in Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `onPanStart` callback function fires when a pan gesture begins on the element. It provides the triggering `PointerEvent` and an `info` object with gesture details, useful for initializing pan-related logic.

```javascript
<motion.div onPanStart={(event, info) => console.log(info.delta.x)} />
```

--------------------------------

### Configure Motion Components with MotionConfig

Source: https://motion.dev/docs/react-motion-config

Import and use MotionConfig to wrap motion components and apply global transition settings. The component accepts a transition prop that serves as a fallback for all child motion components. In this example, a 1-second duration is applied globally to the motion.div animation.

```jsx
import { motion, MotionConfig } from "motion/react"

export const MyComponent = ({ isVisible }) => (
  <MotionConfig transition={{ duration: 1 }}>
    <motion.div
      initial={{ opacity: 0 }}
      animate={{ opacity: 1 }}
    />
  </MotionConfig>
)
```

--------------------------------

### AnimateNumber with Spring Transition in React

Source: https://motion.dev/docs/react-animate-number

Example showing how to customize AnimateNumber animations using the transition prop with Motion's spring animation type. Demonstrates basic transition configuration.

```jsx
<AnimateNumber transition={{ type: "spring" }}>
  {count}
</AnimateNumber>
```

--------------------------------

### `transform` with multiple input/output range values (JavaScript)

Source: https://motion.dev/docs/transform

This example demonstrates `transform`'s flexibility in handling input and output ranges with more than two values. It illustrates how the function interpolates between multiple defined points, allowing for complex, non-linear mappings across different segments of the input range.

```javascript
const x = [-100, 0, 100, 200]
const opacity = [0, 1, 1, 0]
const transformer = transform(x, opacity)

transformer(-50) // 0.5
transformer(50) // 1
transformer(150) // 0.5
```

--------------------------------

### Utilize `whilePress` and `whileHover` with Variants in Vue

Source: https://motion.dev/docs/vue-gestures

This example illustrates how to use named variants with `whilePress` and `whileHover` props. By defining `variants` on the parent `motion.button` and referencing them, complex animation states can be managed and propagated to child `motion.path` components.

```html
<motion.button
  whilePress="press"
  whileHover="hover"
  :variants="buttonVariants"
>
  <svg>
    <motion.path :variants="iconVariants" />
  </svg>
</motion.button>
```

--------------------------------

### AnimateNumber with Dynamic Counter in React

Source: https://motion.dev/docs/react-animate-number

Complete React component example demonstrating AnimateNumber with state management. Shows how to animate number changes when a button increments the count value.

```jsx
import { AnimateNumber } from "motion-plus/react"

function Counter() {
  const [count, setCount] = useState(0)

  return (
    <>
      <button onClick={() => setCount(count + 1)}>Increment</button>
      <AnimateNumber>{count}</AnimateNumber>
    </>
  )
}
```

--------------------------------

### Handle Tap Start Event with `onTapStart` Callback in Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `onTapStart` callback function is invoked when a pointer begins pressing the component. It provides the triggering `PointerEvent` object, useful for custom tap-start logic.

```javascript
<motion.div onTapStart={(event) => console.log(event)} />
```

--------------------------------

### Migrate Layout Animations from Motion 1 to Motion 2

Source: https://motion.dev/docs/react-upgrade-guide

Shows the API migration for layout animations in Motion 2, replacing deprecated `layoutTransition` and `positionTransition` props with the unified `layout` prop. The new approach uses the standard `transition` prop for configuration instead of inline transition arguments.

```jsx
// Before (Motion 1)
<motion.div layoutTransition />

// After (Motion 2)
<motion.div layout />
```

```jsx
// Before (Motion 1)
<motion.div layoutTransition={{ duration: 2 }} />

// After (Motion 2)
<motion.div layout transition={{ duration: 2 }} />
```

--------------------------------

### Create a basic `transform` motion value with `useMotionTemplate` (React)

Source: https://motion.dev/docs/react-use-motion-template

This example demonstrates the fundamental usage of `useMotionTemplate` in React to combine a `useMotionValue` (`x`) into a dynamic CSS `transform` string. The `transform` motion value automatically updates its string content whenever the underlying `x` motion value changes.

```javascript
const x = useMotionValue(100)
const transform = useMotionTemplate`transform(${x}px)`
```

--------------------------------

### Asynchronous Loading of LazyMotion Features (React)

Source: https://motion.dev/docs/react-lazy-motion

This example illustrates how to asynchronously load `LazyMotion` features, which can be beneficial for optimizing initial page load and hydration. It involves creating a separate file for feature export and then dynamically importing it within the `LazyMotion` component's `features` prop.

```jsx
// features.js
import { domAnimation } from "motion/react"
export default domAnimation
  
// index.js
const loadFeatures = () => import("./features.js")
  .then(res => res.default)

function Component() {
  return (
    <LazyMotion features={loadFeatures}>
      <m.div animate={{ scale: 1.5 }} />
    </LazyMotion>
  )
}
```

--------------------------------

### Integrate `delay` with Motion's animation frame loop

Source: https://motion.dev/docs/delay

This example demonstrates how `delay` callbacks execute during the `read` step of Motion's animation loop. It shows how to use `frame.render` to batch write operations, ensuring that DOM modifications are performed efficiently and in sync with the animation frame.

```javascript
import { delay, frame } from "motion"

delay(() => {
  const { left } = element.getBoundingClientRect()

  // Will render later during this animation frame
  frame.render(() => {
    element.style.left = `${left * 2}px`
  })
}, 1)
```

--------------------------------

### Handle hover start and end events with Motion

Source: https://motion.dev/docs/hover

Return a callback from the hover start function to handle the hover end event. The end callback receives the triggering PointerEvent.

```javascript
hover("a", () => {
  console.log("hover start")
  
  return (endEvent) => {
    console.log("hover end")
  }
})
```

--------------------------------

### Animating to a Responsive Value from CSS Variables (React/Tailwind CSS)

Source: https://motion.dev/docs/react-tailwind

Building on the responsive initial values, this code shows how to animate a property (like 'y') to a target value (0) from a starting point defined by a responsive CSS variable. This allows for animations that adapt their starting position based on screen size.

```html
animate={{ opacity: 1, y: 0 }}
```

--------------------------------

### Initiate drag from pointer event

Source: https://motion.dev/docs/vue-use-drag-controls

Start a drag session from any element's onPointerDown event using the controls.start() method. This allows dragging to be triggered from elements other than the motion component itself.

```vue
<template>
<div @pointerdown="(event) => controls.start(event)" />
</template>
```

--------------------------------

### Importing MotionConfig Component in Vue

Source: https://motion.dev/docs/vue-motion-config

This snippet demonstrates how to import the `motion` and `MotionConfig` components from the `motion-v` library within a Vue `<script setup>` block. This is a prerequisite for using `MotionConfig` to configure child `motion` components.

```javascript
import { motion, MotionConfig } from "motion-v"
```

--------------------------------

### Animating React Components with useAnimationFrame Hook

Source: https://motion.dev/docs/react-use-animation-frame

This section provides examples of using the `useAnimationFrame` hook from `motion/react` to create continuous animations in React components. It demonstrates both a concise callback usage and a full functional component integration, illustrating how to leverage `time` and `delta` arguments for dynamic visual effects.

```javascript
useAnimationFrame((time) => {
ref.current.style.transform = `rotateY(${time}deg)`
})
```

```jsx
import { useAnimationFrame } from "motion/react"

function Component() {
const ref = useRef(null)
useAnimationFrame((time, delta) => {
ref.current.style.transform = `rotateY(${time}deg)`
})

return <div ref={ref} />
}
```

--------------------------------

### Detect press start with callback

Source: https://motion.dev/docs/press

Attach a press gesture listener to an element or CSS selector. The callback fires when a press gesture starts and receives the element and PointerEvent as arguments.

```javascript
press("button", (element) => {
  console.log("press started on", element)

  return () => console.log("press ended")
})
```

--------------------------------

### Handle Motion Value Events in React with useMotionValueEvent

Source: https://motion.dev/docs/react-use-motion-value-event

This example demonstrates the `useMotionValueEvent` hook in a React component to listen for `animationStart` and `change` events on a `useMotionValue`. It showcases how to log event occurrences and the latest value, with automatic cleanup of handlers upon component unmount.

```javascript
function Component() {
  const x = useMotionValue(0)
  
  useMotionValueEvent(x, "animationStart", () => {
    console.log("animation started on x")
  })
  
  useMotionValueEvent(x, "change", (latest) => {
    console.log("x changed to", latest)
  })
  
  return <motion.div style={{ x }} />
}
```

--------------------------------

### SDK Function: toShareQueryString

Source: https://motion.dev/docs/studio-sdk-state

Serializes a `TransitionState` object into a URL query string, enabling shareable configuration links.

```APIDOC
## toShareQueryString

### Description
Serialises a `TransitionState` object into a URL query string.

### Method
Function Call

### Endpoint
N/A

### Parameters
#### Function Parameters
- **state** (TransitionState) - Required - The `TransitionState` object to serialize.

### Request Example
```json
{
  "type": "spring",
  "easing": {
    "duration": 0.5,
    "ease": [0.25, 0.1, 0.25, 1]
  },
  "spring": {
    "duration": 0.8,
    "bounce": 0.2,
    "stiffness": 100,
    "damping": 10,
    "mass": 1,
    "type": "physics",
    "isVisualDuration": true
  }
}
```

### Response
#### Success Response (String)
- **queryString** (string) - The URL query string representation of the `TransitionState`.

#### Response Example
```json
"transition=%7B%22type%22%3A%22spring%22%2C%22easing%22%3A%7B%22duration%22%3A0.5%2C%22ease%22%3A%5B0.25%2C0.1%2C0.25%2C1%5D%7D%2C%22spring%22%3A%7B%22duration%22%3A0.8%2C%22bounce%22%3A0.2%2C%22stiffness%22%3A100%2C%22damping%22%3A10%2C%22mass%22%3A1%2C%22type%22%3A%22physics%22%2C%22isVisualDuration%22%3Atrue%7D%7D"
```
```

--------------------------------

### Implement scroll-triggered animations with useAnimate and useInView in Vue

Source: https://motion.dev/docs/vue-use-animate

This example combines `useAnimate` with `useInView` to trigger animations when the scoped element enters the viewport. It uses a `watch` effect to detect changes in `isInView` and applies an animation to the `scope.value` element when it becomes visible.

```vue
<script setup>
import { useAnimate, useInView } from 'motion-v'

const [scope, animate] = useAnimate()
const isInView = useInView(scope)

watch(isInView, (inView) => {
  if (inView) {
    animate(scope.value, { opacity: 1 })
  }
})
</script>

<template>
  <ul ref="scope">
    <li />
    <li />
    <li />
  </ul>
</template>
```

--------------------------------

### Set and Get Motion Value State

Source: https://motion.dev/docs/react-motion-value

Demonstrates updating a motion value using the set() method and retrieving its current state with the get() method. Updates to motion values do not trigger React re-renders and are batched to the next animation frame.

```javascript
const x = useMotionValue(0)

// Update motion value
x.set(100)

// Read current state
x.get() // 100
```

--------------------------------

### Delay a callback using Motion's `delay` function

Source: https://motion.dev/docs/delay

This example shows how to schedule a callback function to execute after a specified duration, measured in seconds. The callback will fire on the next animation frame once the duration has passed, ensuring synchronization with Motion's animation loop.

```javascript
delay(() => console.log("one second!"), 1)
```

--------------------------------

### Handle onDragStart callback

Source: https://motion.dev/docs/react-motion-component

Callback function that fires when a drag gesture starts. Receives the triggering PointerEvent and info object containing delta, offset, point, and velocity properties.

```JSX
<motion.div drag onDragStart={(event, info) => console.log(info.delta.x)} />
```

--------------------------------

### Read Motion Value State with get Method

Source: https://motion.dev/docs/vue-motion-value

Retrieve the current state of a motion value using the get method. Returns the latest numeric or string value held by the motion value.

```javascript
x.get() // 100
```

--------------------------------

### Set Animation Sequence Timing to Specific Time

Source: https://motion.dev/docs/animate

Uses the 'at' parameter with a numeric value to start an animation at a specific time (in seconds) from the sequence start. Overrides default sequential timing to enable precise temporal control.

```javascript
const sequence = [
  ["nav", { opacity: 1 }],
  
  // This will start 0.5 from the start of the whole animation:
  ["nav", { x: 100 }, { at: 0.5 }],
]
```

--------------------------------

### Defining Input and Output Ranges for `useTransform` (React)

Source: https://motion.dev/docs/react-use-transform

Illustrates how to define `input` and `output` arrays for `useTransform`'s value mapping. This example maps an `x` value from -100 to 100 to an opacity range of 0 to 1 to 0, creating a fade-in/fade-out effect.

```javascript
const input = [-100, 0, 100]
const output = [0, 1, 0]
```

--------------------------------

### Animation Controls - Promise-based Completion

Source: https://motion.dev/docs/upgrade-guide

Demonstrates the new promise-based API for detecting animation completion. The `finished` property has been removed and replaced with native promise support, allowing animations to be awaited or chained with `.then()` callbacks.

```javascript
const animation = animate()

animation.then(() => {})
await animation
```

--------------------------------

### Basic Ticker Component Setup - React

Source: https://motion.dev/docs/react-ticker

Creates a simple ticker animation with an array of React nodes. The component accepts an items prop containing valid React nodes (components, strings, or numbers) and renders them in a continuously scrolling animation.

```jsx
<Ticker items={items} />
```

--------------------------------

### Dynamic `useTransform` with `useTime` for Animation (React)

Source: https://motion.dev/docs/react-use-transform

Demonstrates how `useTransform` can create a continuously animating motion value by subscribing to `useTime`. This example calculates a sine wave-based `y` position, creating an oscillating effect over time.

```javascript
const distance = 100
const time = useTime()
const y = useTransform(() => Math.sin(time.get() / 1000) * distance)
```

--------------------------------

### Animate element on press start and end

Source: https://motion.dev/docs/press

Use the press function to trigger animations on press start and return a function to animate back on press end. Useful for creating interactive button feedback.

```javascript
press("button", (element) => {
  animate(element, { scale: 0.9 })

  return () => animate(element, { scale: 1 })
})
```

--------------------------------

### Getting and Setting Animation Playback Time (JavaScript)

Source: https://motion.dev/docs/animate

The `time` property allows you to get or set the current playback time of the animation in seconds. This can be used to jump to a specific point in the animation or retrieve its current progress.

```javascript
const animation = animate(x, 100, { duration: 1 })

// Set animation time to 0.5 seconds
animation.time = 0.5

// Get animation time
console.log(animation.time) // 0.5
```

--------------------------------

### Setup useDragControls with motion component

Source: https://motion.dev/docs/vue-use-drag-controls

Create drag controls using useDragControls() and pass them to a motion component via the drag-controls prop. The motion component must have the drag prop enabled to work with the controls.

```vue
<script setup>
import { useDragControls, motion } from 'motion-v'

const controls = useDragControls()
</script>

<template>
<motion.div drag :drag-controls="controls" />
</template>
```

--------------------------------

### Initializing a Motion Value `x` (React)

Source: https://motion.dev/docs/react-use-transform

Initializes a `useMotionValue` named `x` with a starting value of 0. This motion value serves as the input for subsequent `useTransform` operations, allowing its value to be mapped or transformed.

```javascript
const x = useMotionValue(0)
```

--------------------------------

### Import and create a derived motionValue in JavaScript

Source: https://motion.dev/docs/transform-value

This snippet shows the basic setup for using `transformValue`, including importing necessary functions from the 'motion' library. It demonstrates creating a new `motionValue` (`doubleX`) that is derived by multiplying another `motionValue` (`x`) by two.

```javascript
import { motionValue, transformValue } from "motion"

const x = motionValue(0)
const doubleX = transformValue(() => x.get() * 2)
```

--------------------------------

### Create layout animations with Radix Tabs

Source: https://motion.dev/docs/radix

Shows how to implement layout animations with Radix Tabs by hoisting state management and using motion.div with the layout prop. Demonstrates optional layoutDependency prop for performance optimization.

```jsx
const [tab, setTab] = useState("account")

return (
  <Tabs.Root value={tab} onValueChange={setTab} asChild>
    <motion.div layout layoutDependency={tab}>
    </motion.div>
  </Tabs.Root>
)
```

--------------------------------

### Set Repeat Type for Animation in Framer Motion

Source: https://motion.dev/docs/vue-transitions

Defines how an animation repeats. Options include `loop` (repeats from start), `reverse` (alternates forward/backward playback), and `mirror` (switches origin/target). Default is `loop`.

```Framer Motion
<motion.div
  :animate="{ rotate: 180 }"
  :transition="{
    repeat: 1,
    repeatType: 'reverse',
    duration: 2
  }"
/>
```

--------------------------------

### Basic `useAnimate` Component in React

Source: https://motion.dev/docs/react-use-animate

This example demonstrates the fundamental usage of `useAnimate` within a React functional component. It shows how to obtain the `scope` ref and `animate` function, attach the `scope` ref to a parent element, and use `animate` within a `useEffect` hook to animate child elements, with automatic cleanup on component unmount.

```javascript
function Component() {
  const [scope, animate] = useAnimate()

  useEffect(() => {
    // This "li" selector will only select children
    // of the element that receives `scope`.
    animate("li", { opacity: 1 })
  })
  
  return <ul ref={scope}>{children}</ul>
}
```

--------------------------------

### React: Creating a perpetual rotation animation with useTime and useTransform

Source: https://motion.dev/docs/react-use-time

This example demonstrates how to use the `useTime` hook to obtain a motion value that updates every frame. This time value is then transformed using `useTransform` to create a continuous rotation animation for a `motion.div` component. The `clamp: false` option ensures the rotation continues indefinitely.

```javascript
const time = useTime();
const rotate = useTransform(time, [0, 4000], [0, 360], { clamp: false });

return <motion.div style={{ rotate }} />
```

--------------------------------

### Basic AnimateActivity Setup with Motion

Source: https://motion.dev/docs/react-animate-activity

Demonstrates the fundamental usage of AnimateActivity with a motion.div child element. The component toggles between 'visible' and 'hidden' modes based on the isVisible state, applying opacity animations on entry and exit.

```jsx
<AnimateActivity mode={isVisible ? "visible" : "hidden"}>
  <motion.div
    initial={{ opacity: 0 }}
    animate={{ opacity: 1 }}
    exit={{ opacity: 0 }}
  />
</AnimateActivity>
```

--------------------------------

### Importing the wrap function in JavaScript

Source: https://motion.dev/docs/wrap

Shows how to import the `wrap` utility function from the 'motion' library in a JavaScript or TypeScript project, making it available for use.

```javascript
import { wrap } from "motion"
```

--------------------------------

### Basic AnimateNumber Usage in React

Source: https://motion.dev/docs/react-animate-number

Simple example showing how to use AnimateNumber component with a static number value. The component accepts a single child which must be a number that will be animated when it changes.

```jsx
<AnimateNumber>300</AnimateNumber>
```

--------------------------------

### Unsubscribing from Motion Value changes in JavaScript

Source: https://motion.dev/docs/motion-value

This example demonstrates how to unsubscribe a listener from a `motionValue`'s 'change' event. The `on` method returns a function that, when called, removes the registered listener, preventing further callbacks.

```javascript
const unsubscribe = x.on("change", latest => console.log(latest))
```

--------------------------------

### Handle Hover Start Event with `onHoverStart` Callback in Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `onHoverStart` callback function is invoked when a pointer begins hovering over the component. It provides the triggering `PointerEvent` object, useful for custom hover-start logic.

```javascript
<motion.div onHoverStart={(event) => console.log(event)} />
```

--------------------------------

### Applying Global Transition with MotionConfig in Vue Template

Source: https://motion.dev/docs/vue-motion-config

This example shows how to use the `MotionConfig` component in a Vue template to apply a global transition property to all child `motion` components. Here, a `duration` of 1 second is set for the transition, and a child `motion.div` animates its opacity from 0 to 1, inheriting this transition.

```html
<MotionConfig :transition="{ duration: 1 }">
<motion.div
:initial="{ opacity: 0 }"
:animate="{ opacity: 1 }"
/>
</MotionConfig>
```

--------------------------------

### Generating Tailwind CSS Spring Easing Utilities with Motion for AI

Source: https://motion.dev/docs/react-tailwind

This example demonstrates how Motion for AI can generate CSS spring animations using the `linear()` easing function, making them reusable as Tailwind utility classes. It provides a `@theme` configuration block that defines several spring easings, such as `ease-spring-snappy` and `ease-spring-soft`.

```css
@theme {
  --ease-spring-snappy: linear(0, 0.2375, 0.5904, 0.8358, 0.9599, 1.0061, 1.0152, 1.0116, 1.0062, 1.0025, 1.0006, 0.9999, 1);
  --ease-spring: linear(0, 0.0942, 0.2989, 0.5275, 0.73, 0.8839, 0.9858, 1.0425, 1.0655, 1.0666, 1.0558, 1.0405, 1.0255, 1.0131, 1.0043, 0.9989, 0.9962, 1);
  --ease-spring-soft: linear(0, 0.0332, 0.1241, 0.2583, 0.4207, 0.5967, 0.7729, 0.9379, 1.0826, 1.2006, 1.2883, 1.3445, 1.3701, 1.3679, 1.3423, 1.2983, 1.2415, 1.1774, 1.1113, 1.0477, 0.9904, 0.9421, 0.9047, 0.8789, 0.8648, 0.8615, 0.8677, 0.8815, 0.9009, 0.9239, 0.9485, 0.9727, 0.9952, 1.0146, 1.0303, 1.0417, 1.0487, 1.0515, 1.0506, 1.0465, 1.0401, 1.032, 1.023, 1.0138, 1.0051, 0.9974, 0.9909, 0.986, 0.9828, 0.9811, 0.9809, 0.9819, 0.984, 0.9868, 0.99, 0.9935, 0.9968, 0.9998, 1.0025, 1.0045, 1.006, 1.0069, 1.0072, 1.0069, 1.0063, 1.0054, 1.0042, 1.003, 1.0017, 1.0005, 0.9995, 0.9986, 0.998, 0.9976, 1);
}
```

--------------------------------

### Getting the current state of a Motion Value in JavaScript

Source: https://motion.dev/docs/motion-value

This code shows how to retrieve the current, latest value of a `motionValue` using the `.get()` method. This is useful for reading the value at any given point in time.

```javascript
const latest = x.get() // 100
```

--------------------------------

### Imperative GSAP Integration in React using `useGSAP`

Source: https://motion.dev/docs/gsap-vs-motion

This example illustrates how GSAP, with its imperative model, integrates into React components using the `useGSAP` hook and refs. While `useGSAP` helps manage lifecycle, the imperative nature of GSAP often leads to more verbose and potentially error-prone code when mixed with React's declarative paradigm.

```jsx
const container = useRef()

useGSAP(() => {
  gsap.to(".box", { x: 100 })
}, { scope: container })

return (
  <div ref={container}>
    <div className="box"></div>
  </div>
);
```

--------------------------------

### Use `spring` animation type with Motion.dev Mini `animate`

Source: https://motion.dev/docs/animate

Shows how to use the `spring` animation type with the `motion/mini` version of `animate`. This example imports `spring` from `motion` and applies it with specific stiffness for physics-based animation.

```javascript
import { animate } from "motion/mini"
import { spring } from "motion"

animate(
  element,
  { transform: "translateX(100px)" },
  { type: spring, stiffness: 300 }
)
```

--------------------------------

### Optimize Motion Vue Layout Animations with `layoutDependency`

Source: https://motion.dev/docs/vue-radix

This example demonstrates how to improve the performance of layout animations by explicitly providing a `layoutDependency` to the `motion.div` component. By passing the `tab` state variable, Motion knows exactly which dependency to track for layout changes, leading to more efficient animations.

```Vue
<motion.div layout :layoutDependency="tab">

```

--------------------------------

### Control Animation Frame with usePageInView

Source: https://motion.dev/docs/react-use-page-in-view

Start or stop animation loops created with useAnimationFrame based on page visibility. Passes the update function when page is in view, undefined when hidden to pause animations.

```javascript
useAnimationFrame(isPageInView ? update : undefined)
```

--------------------------------

### dragTransition

Source: https://motion.dev/docs/react-motion-component

Customizes the 'inertia' animation that starts when releasing a draggable element, based on dragging velocity.

```APIDOC
## dragTransition

### Description
Allows you to change dragging momentum transition. When releasing a draggable element, an animation with type `"inertia"` starts. The animation is based on your dragging velocity. This property allows you to customize it.

### Type
`object`

### Parameters
- **bounceStiffness** (number) - Optional - Stiffness of the bounce animation.
- **bounceDamping** (number) - Optional - Damping of the bounce animation.

### Usage Example
```jsx
<motion.div
  drag
  dragTransition={{ bounceStiffness: 600, bounceDamping: 10 }}
/>
```
```

--------------------------------

### Apply Exit Animations to Radix Tooltip with Motion Vue and `AnimatePresence`

Source: https://motion.dev/docs/vue-radix

This comprehensive example demonstrates how to use `AnimatePresence` to enable exit animations for a Radix Tooltip component. By wrapping the `Tooltip.Content` (which uses `as-child` to render a `motion.div`) with `AnimatePresence`, the tooltip's content can animate out when it unmounts.

```Vue
 <Tooltip.Provider>
        <Tooltip.Root>
          <Tooltip.Trigger class="tooltip-trigger">
              Hover or focus
          </Tooltip.Trigger>
          <Tooltip.Portal>
            <AnimatePresence>
              <Tooltip.Content as-child :side-offset="10">
                <motion.div
                  class="tooltip-content"
                  :initial="{ opacity: 0, y: 20, scale: 0.8 }"
                  :animate="{ opacity: 1, y: 0, scale: 1 }"
                  :exit="{ opacity: 0,y: 20,}"
                >
                  Add to library
                  <Tooltip.Arrow class="tooltip-arrow" />
                </motion.div>
              </Tooltip.Content>
            </AnimatePresence>
          </Tooltip.Portal>
        </Tooltip.Root>
  </Tooltip.Provider>
```

--------------------------------

### time Property

Source: https://motion.dev/docs/animate

Gets and sets the current playback time of the animation. Allows you to seek to a specific point in the animation timeline.

```APIDOC
## time Property

### Description
Gets and sets the current time of the animation. Use this to seek to a specific point or retrieve the current playback position.

### Property
- **time** (number) - Get/Set - Current animation time in seconds

### Usage Example
```javascript
const animation = animate(x, 100, { duration: 1 })

// Set animation time to 0.5 seconds
animation.time = 0.5

// Get animation time
console.log(animation.time) // 0.5
```
```

--------------------------------

### Detect drag gesture start with onDragStart callback

Source: https://motion.dev/docs/vue-motion-component

The onDragStart callback fires when a drag gesture begins. It provides the triggering PointerEvent and info object with delta, offset, point, and velocity properties.

```vue
<motion.div drag @dragStart="(event, info) => console.log(info.delta.x)" />
```

--------------------------------

### Synchronously loading `domAnimation` features with `LazyMotion` in Vue

Source: https://motion.dev/docs/vue-lazymotion

Illustrates how to bundle animation features directly into the main JavaScript bundle. This involves importing `LazyMotion` and a feature package like `domAnimation` in the script setup and then passing the feature package directly to the `features` prop of `LazyMotion` in the template.

```javascript
<script setup>
import { LazyMotion, domAnimation, m } from "motion-v"
</script>
```

```html
<template>  
  <LazyMotion :features="domAnimations">
    <m.div :animate="{ opacity: 1 }" />
  </LazyMotion>
</template>
```

--------------------------------

### cancel() Method

Source: https://motion.dev/docs/animate

Cancels the animation and reverts all animated values back to their initial state before the animation started.

```APIDOC
## cancel() Method

### Description
Cancels the animation, reverting it to the initial state.

### Method
- **cancel()** - Stops animation and reverts to initial values

### Usage Example
```javascript
const animation = animate(element, { opacity: 0 })
animation.cancel()
```
```

--------------------------------

### Control animations with Motion hover

Source: https://motion.dev/docs/hover

Use hover callbacks to start and control animations. Return a cleanup function to stop animations when hover ends.

```javascript
hover("li", (element) => {
  const animation = animate(element, { rotate: 360 })
  
  return () => animation.stop()
})
```

--------------------------------

### speed Property

Source: https://motion.dev/docs/animate

Gets and sets the current playback speed of the animation. Supports normal playback, slow motion, fast-forward, and reverse playback.

```APIDOC
## speed Property

### Description
Gets and sets the current playback speed of the animation.

### Speed Values
- `1` - Normal playback rate
- `0.5` - Half speed (slow motion)
- `2` - Double speed (fast-forward)
- `-1` - Reverse playback

### Property
- **speed** (number) - Get/Set - Playback speed multiplier

### Usage Example
```javascript
const animation = animate(element, { opacity: 0 })

const currentSpeed = animation.speed

// Double current speed
animation.speed = currentSpeed * 2
```
```

--------------------------------

### Reverse an Easing Function with `reverseEasing` Modifier

Source: https://motion.dev/docs/easing-functions

This example explains how to use the `reverseEasing` modifier to create a new easing function that is the inverse of an existing one. For instance, an 'easeIn' function can be transformed into an 'easeOut' function, effectively reversing its acceleration profile.

```javascript
import { reverseEasing } from "motion"

const powerIn = (progress) => progress * progress

const powerOut = reverseEasing(powerIn)
```

--------------------------------

### Animate a React Three Fiber component with Framer Motion 3D

Source: https://motion.dev/docs/react-three-fiber

This example demonstrates how to use a `motion` component, specifically `motion.pointLight`, to animate its `x` position. By replacing standard R3F components with their `motion` equivalents, you can apply animation props like `animate` directly.

```jsx
<motion.pointLight animate={{ x: 2 }} />
```

--------------------------------

### Import resize function from Motion library

Source: https://motion.dev/docs/resize

Import the resize function from the Motion library to enable size change monitoring capabilities in your application.

```JavaScript
import { resize } from "motion"
```

--------------------------------

### Snap motion component to cursor position

Source: https://motion.dev/docs/react-use-drag-controls

Configure the drag gesture to immediately snap the motion component to the cursor position by passing snapToCursor: true option to the start method.

```javascript
controls.start(event, { snapToCursor: true })
```

--------------------------------

### Apply Staggered Duration to ScrambleText in React

Source: https://motion.dev/docs/react-scramble-text

Illustrates how to use Motion's `stagger` function with the `duration` prop to create a character-by-character reveal effect. This example includes a `startDelay` to control when the scrambling begins.

```jsx
import { stagger } from "motion"
import { ScrambleText } from "motion-plus/react"

// Start scrambling at the same time, reveal after 1
// second, with a 0.05 delay between each character/
<ScrambleText duration={stagger(0.05, { startDelay: 1 })} >
  Hello world!
</ScrambleText>
```

--------------------------------

### Define Initial Velocity for Spring Animation in Framer Motion

Source: https://motion.dev/docs/vue-transitions

Specifies the initial velocity of the spring animation. This property influences the starting momentum of the animation. Default is the current value's velocity.

```Framer Motion
<motion.div
  :animate="{ rotate: 180 }"
  :transition="{ type: 'spring', velocity: 2 }"
/>
```

--------------------------------

### Creating and using a `transformer` function (JavaScript)

Source: https://motion.dev/docs/transform

This snippet shows how to create a reusable transformation function by providing an input and an output range to `transform`. The resulting `transformer` function can then be called with an input value to get its corresponding mapped output, adhering to the specified range constraints.

```javascript
const transformer = transform([0, 100], [0, 360])

transformer(50) // 180
```

--------------------------------

### useInView with Initial Value Option in React

Source: https://motion.dev/docs/react-use-in-view

Shows how to set an initial return value using the initial option. This is useful for server-side rendering or when you want to assume an element is in view before measurement occurs, preventing layout shifts.

```javascript
import { useInView } from "motion/react"
import { useRef } from "react"

function Component() {
  const ref = useRef(null)
  const isInView = useInView(ref, { initial: true })
  
  return <div ref={ref} />
}
```

--------------------------------

### Glide Animation with Target Modification

Source: https://motion.dev/docs/glide

Demonstrates the changeTarget option which allows intercepting and modifying the automatically calculated animation target. The example snaps the target to the nearest 100-unit increment.

```javascript
const roundTo = 100

glide({
  changeTarget: (target) => Math.ceil(target / roundTo) * roundTo
})
```

--------------------------------

### Connecting `springValue` to a `motionValue` for Dynamic Animation in JavaScript

Source: https://motion.dev/docs/spring-value

This example illustrates how to create a `springValue` that automatically tracks and animates changes from another `motionValue`. It sets up a `pointerX` `motionValue` to capture mouse coordinates, and the `springValue` `x` then smoothly animates to these `pointerX` updates. The resulting animated value is applied to a `div`'s style.

```javascript
const pointerX = motionValue(0)
const x = springValue(pointerX)

document.addEventListener("pointerMove", (e) => {
  // x will animate these changes with a spring animation
  pointerX.set(e.clientX)
})

styleEffect("div", { x })
```

--------------------------------

### Create infinite looping SVG draw animation with `pathOffset` (JavaScript)

Source: https://motion.dev/docs/svg-effect

This example shows how to achieve an infinite looping draw animation by animating `pathOffset` from `0` to `1`. When `pathSpacing` is left unset, `svgEffect` dynamically calculates it to ensure a seamless, continuous loop.

```JavaScript
const pathLength = motionValue(0.5)
const pathOffset = motionValue(0)

svgEffect("path", { pathLength, pathOffset })

animate(pathOffset, [0, 1], { repeat: Infinity })
```

--------------------------------

### Observe changes in derived motionValue in JavaScript

Source: https://motion.dev/docs/transform-value

This example highlights the automatic dependency tracking of `transformValue`. When the source `motionValue` (`x`) is updated, the derived `motionValue` (`doubleX`) automatically recomputes its value and triggers its 'change' event, logging the new value.

```javascript
doubleX.on("change", (latest) => console.log(latest))

x.set(10) // doubleX will log 20
```

--------------------------------

### Getting Animation Duration (JavaScript)

Source: https://motion.dev/docs/animate

The `duration` property returns the read-only duration of a single iteration of the animation. This value does not include any delays or repeat options.

```javascript
const animation = animate(element, { opacity: 0 })

const duration = animation.duration
```

--------------------------------

### Importing `springValue` and Initializing with Various Number Formats in JavaScript

Source: https://motion.dev/docs/spring-value

This code demonstrates the basic import of `springValue` from the 'motion' library. It shows how to initialize `springValue` instances with both plain numerical values and string-based values that include units, such as '1turn' for rotation.

```javascript
import { springValue } from "motion"

const scaleX = springValue(0)
const rotate = springValue("1turn")
```

--------------------------------

### Chaining `springValue` with `mapValue` and `motionValue` in JavaScript

Source: https://motion.dev/docs/spring-value

This advanced example demonstrates how `springValue` can be used in conjunction with `motionValue` and `mapValue`. An `opacity` `motionValue` is mapped to a new range for `x`, and then `springValue` is applied to `x`, creating a spring animation based on the mapped `opacity` changes.

```javascript
const opacity = motionValue(1)
const x = mapValue(opacity, [0, 1], [0, 100])
const xWithSpring = springValue(x)
```

--------------------------------

### Scroll Callback Signature Update

Source: https://motion.dev/docs/upgrade-guide

Shows the updated scroll function callback signature that now accepts two arguments: `progress` and `info`. The new signature allows callbacks using only `progress` to run via native ScrollTimeline, improving performance by reducing scroll measurements.

```javascript
// Previously
scroll((info) => {}, options)

// Now
scroll((progress, info) => {}, options)
```

--------------------------------

### Animating combined transform property for hardware acceleration with Motion

Source: https://motion.dev/docs/performance

This JavaScript example shows how to animate an element's `transform` property directly using the Motion library. By combining transform functions into a single `transform` string, this approach is recommended when hardware acceleration is crucial, as it is more likely to be offloaded to the compositor/GPU compared to animating individual transform properties via CSS variables.

```javascript
animate(".box", { transform: "translateX(100px) scale(2)" })
```

--------------------------------

### Configure Spring Initial Velocity Parameter

Source: https://motion.dev/docs/animate

Sets the initial velocity of spring animations. The default uses the current value velocity. This parameter determines the starting speed of the animation before spring physics take effect.

```javascript
animate(
  ".my-element",
  { rotate: 180 },
  { type: "spring", velocity: 2 }
)
```

--------------------------------

### Set Minimum Constraint for Inertia Animation in Framer Motion

Source: https://motion.dev/docs/vue-transitions

Defines a minimum boundary for an inertia animation. If the animation value attempts to go below this, it will 'bump' against it or spring to it if the animation starts below this value. Used in conjunction with `max`.

```Framer Motion
<motion.div
  drag
  :dragTransition="{ min: 0, max: 100 }"
/>
```

--------------------------------

### Basic usePageInView Hook Usage

Source: https://motion.dev/docs/react-use-page-in-view

Use the usePageInView hook to get a boolean state indicating whether the current page is in view. Returns true when the page is active, defaults to true on server and initial client render.

```javascript
const isPageInView = usePageInView()
```

--------------------------------

### Update Framer Motion 3D imports to version 6.0

Source: https://motion.dev/docs/react-upgrade-guide

Migrate from the legacy framer-motion/three import path to the new dedicated framer-motion-3d package. This change consolidates 3D functionality into a separate package for better modularity and maintenance.

```javascript
// Before (v5.x and earlier)
import { /* 3D components */ } from "framer-motion/three"

// After (v6.0+)
import { /* 3D components */ } from "framer-motion-3d"
```

--------------------------------

### Apply Press Gesture Animation with `whilePress` in Vue

Source: https://motion.dev/docs/vue-gestures

This example demonstrates the `whilePress` prop on a `motion.button` to apply animations when the primary pointer presses down and releases on the component. It animates both `scale` and `rotate` properties during the press gesture.

```html
<motion.button :whilePress="{ scale: 0.9, rotate: 3 }" />
```

--------------------------------

### Apply multiple MotionValues to SVG styles with `svgEffect` (JavaScript)

Source: https://motion.dev/docs/svg-effect

This example demonstrates how `svgEffect` can accept a map of multiple `motionValue` instances, each controlling a different style or attribute of an SVG element. Here, `strokeWidth` and `stroke` are animated simultaneously on a 'circle' element.

```JavaScript
const stroke = motionValue("#00f")
const strokeWidth = motionValue(5)

svgEffect("circle", { strokeWidth, stroke })
```

--------------------------------

### useMotionValueEvent - Basic Setup in Vue

Source: https://motion.dev/docs/vue-use-motion-value-event

Demonstrates basic usage of useMotionValueEvent to listen to motion value changes and animation events in a Vue component. The composable automatically cleans up event handlers when the component unmounts, preventing memory leaks.

```vue
<script setup>
import { useMotionValue, useMotionValueEvent } from "motion-v"
const x = useMotionValue(0)
useMotionValueEvent(x, "animationStart", () => {
  console.log("animation started on x")
})
useMotionValueEvent(x, "change", (latest) => {
  console.log("x changed to", latest)
})
</script>

<template>
  <motion.div :style="{ x }" />
</template>
```

--------------------------------

### Combine multiple motion values for CSS `filter` with `useMotionTemplate` (React)

Source: https://motion.dev/docs/react-use-motion-template

This example showcases `useMotionTemplate`'s ability to combine multiple `useMotionValue` instances (`blur`, `saturate`) with static text to construct a dynamic CSS `filter` property. The resulting `filter` motion value is then directly applied to a `motion.div`'s `style` prop, updating automatically as `blur` or `saturate` change.

```javascript
const blur = useMotionValue(10)
const saturate = useMotionValue(50)
const filter = useMotionTemplate`blur(${10}px) saturate(${saturate}%)`

return <motion.div style={{ filter }} />
```

--------------------------------

### Define a callback with custom keyframes in Motion.dev

Source: https://motion.dev/docs/animate

Shows how to pass custom keyframes to a callback function within an animation sequence. The callback will receive values from the specified keyframes, such as color values in this example.

```javascript
const sequence = [
  [(color) => console.log(color), ["#000", "#fff"]]
]
```

--------------------------------

### Apply Staggered Delay to scrambleText Animation

Source: https://motion.dev/docs/scramble-text

Shows how to use `stagger()` with the `delay` option in `scrambleText` to make characters start scrambling one by one. All characters then reveal after a fixed duration, creating a sequential scrambling effect.

```javascript
// Chars start scrambling one-by-one, all reveal after 1s
scrambleText(element, {
  delay: stagger(0.1),
  duration: 1
})
```

--------------------------------

### Implementing Scroll-Triggered Animations with `useAnimate` and `useInView` in React

Source: https://motion.dev/docs/react-use-animate

This code illustrates how to combine `useAnimate` with `useInView` to create animations that trigger when a component scrolls into the viewport. The `useEffect` hook listens for changes in `isInView` to start an animation on the scoped element, providing a common pattern for interactive scroll effects.

```javascript
import { useAnimate, useInView } from "motion/react"

function Component() {
  const [scope, animate] = useAnimate()
  const isInView = useInView(scope)
  
  useEffect(() => {
     if (isInView) {
       animate(scope.current, { opacity: 1 })
     }
  }, [isInView])
  
  return (
    <ul ref={scope}>
      <li />
      <li />
      <li />
    </ul>
  )
}
```

--------------------------------

### Basic Hover Animation with Motion and Tailwind CSS (React)

Source: https://motion.dev/docs/react-tailwind

This example demonstrates how to create a basic interactive button using Tailwind CSS for styling and Motion for animation. Tailwind handles the static appearance, while Motion's `whileHover` and `whileTap` props manage the interactive scaling effects.

```javascript
import { motion } from "motion/react";
  
function Button() {
return (
<motion.button
className="px-6 py-3 bg-indigo-600 text-white font-semibold rounded-lg shadow-lg"
whileHover={{ scale: 1.1 }}
whileTap={{ scale: 0.9 }}
>
Click Me!
</motion.button>
);
}
```

--------------------------------

### Import Motion for React in Framer

Source: https://motion.dev/docs/framer

This snippet demonstrates how to import the `motion` component and `useSpring` hook from the `framer-motion` library for use in Framer code components or overrides. It clarifies that `framer-motion` should be used instead of `motion/react` as per Motion documentation.

```javascript
import { motion, useSpring } from "framer-motion"
```

--------------------------------

### Detailed `useTransform` with Transform Function (React)

Source: https://motion.dev/docs/react-use-transform

Provides a specific example of `useTransform` using a transform function to double a motion value `x`. This highlights how the function dynamically calculates a new value based on `x`'s current state, updating on each change.

```javascript
const doubledX = useTransform(() => x.get() * 2)
```

--------------------------------

### Implement Basic Exit Animations with Motion Vue's `AnimatePresence`

Source: https://motion.dev/docs/vue-radix

This example illustrates the fundamental usage of Motion Vue's `AnimatePresence` component. It wraps a conditionally rendered `Motion` component, allowing `AnimatePresence` to detect when the `Motion` component is unmounting and trigger its `exit` animation.

```Vue
<template>
  <AnimatePresence>
    <Motion
      v-if="isOpen"
      :exit="{ opacity: 0 }"
    />
  </AnimatePresence>
</template>
```

--------------------------------

### resize - Viewport Monitoring

Source: https://motion.dev/docs/resize

Monitor viewport size changes by passing a callback function to resize. The callback receives an object with width and height getters that provide the current viewport dimensions.

```APIDOC
## resize(callback)

### Description
Monitor and react to viewport size changes using a callback function.

### Method
Function

### Signature
```javascript
resize(callback: (dimensions: { width: number, height: number }) => void): () => void
```

### Parameters
#### Callback Function
- **callback** (function) - Required - Function invoked when viewport size changes. Receives an object with width and height getters.

### Request Example
```javascript
import { resize } from "motion"

// Basic viewport monitoring
resize(() => console.log("viewport change detected"))

// With dimension access
resize(({ width, height }) => console.log(width, height))
```

### Response
#### Return Value
- **stop** (function) - A cleanup function that removes the attached listener when called.

### Response Example
```javascript
const stop = resize(({ width, height }) => {
  console.log("Viewport size:", width, height)
})

// Later, remove the listener
stop()
```

### Notes
- All resize handlers are triggered via a single, shared ResizeObserver for optimal performance.
- The callback is called whenever the viewport dimensions change.
- Width and height are provided as getters for lazy evaluation.
```

--------------------------------

### Customize dragTransition inertia animation

Source: https://motion.dev/docs/react-motion-component

Allows customization of the inertia animation that starts when a draggable element is released. Configure properties like bounceStiffness and bounceDamping to adjust the momentum-based animation behavior.

```JSX
<motion.div
  drag
  dragTransition={{ bounceStiffness: 600, bounceDamping: 10 }}
/>
```

--------------------------------

### Apply Motion Values to Object Properties with propEffect

Source: https://motion.dev/docs/prop-effect

propEffect connects motion values to object properties, automatically updating them each animation frame. This example demonstrates applying a motion value to a position object and then updating it with set() and animate() methods.

```javascript
const pos = { x: 0, y: 0, z: 0 }
const x = motionValue(0)

propEffect(pos, { x })

// Set x on pos to 100
x.set(100)

// Animate x on pos to 200
animate(x, 200)
```

--------------------------------

### Instantiate TransitionState Object in Motion Studio

Source: https://motion.dev/docs/studio-sdk-state

This snippet demonstrates how to import and create a new `TransitionState` object from the 'motion-studio' library. The `TransitionState` manages animation options, including both easing and spring configurations, allowing for easy switching between types without losing state.

```typescript
import { TransitionState } from "motion-studio"

const state = new TransitionState()
```

--------------------------------

### Handle press start and end events

Source: https://motion.dev/docs/press

Return a function from the press callback to handle the press end event. The returned function is called when the press gesture completes or is cancelled.

```javascript
press(element, (element, startEvent) => {
  console.log("press start")
  
  return (endEvent) => {
    console.log("press end")
  }
})
```

--------------------------------

### Destructuring `useAnimate` Hook Return Values in React

Source: https://motion.dev/docs/react-use-animate

This example shows how `useAnimate` returns a tuple containing a `scope` ref and an `animate` function. These are typically destructured directly when calling the hook, providing convenient access to the scoped animation capabilities.

```javascript
function Component() {
  const [scope, animate] = useAnimate()
}
```

--------------------------------

### Replace motion.custom() with motion() and forwardMotionProps in Framer Motion 4.0

Source: https://motion.dev/docs/react-upgrade-guide

Migrate from the deprecated motion.custom() method to motion() with the forwardMotionProps option to forward all Framer Motion props to underlying components. This change simplifies the API and improves consistency.

```javascript
// Before (v3.x)
const MotionComponent = motion.custom(Component)

// After (v4.0+)
const MotionComponent = motion(Component, {
    forwardMotionProps: true
})
```

--------------------------------

### Adjust Keyframe Timing with 'times' in Motion (Vue)

Source: https://motion.dev/docs/vue-transitions

This example demonstrates using the `times` property to control the position of keyframes throughout an animation. Each value in the `times` array, between 0 and 1, maps to a corresponding keyframe, allowing precise control over when each keyframe value is reached during the animation's duration.

```vue
<motion.div
  :animate="{
    x: [0, 100, 0],
    transition: { times: [0, 0.3, 1] }
  }"
/>
```

--------------------------------

### Importing `useAnimate` from Motion React

Source: https://motion.dev/docs/react-use-animate

This snippet illustrates the different ways to import the `useAnimate` hook from the Motion library in React. Developers can choose between the 'mini' bundle for a smaller footprint or the full 'react' bundle for all features, depending on their project requirements.

```javascript
// Mini
import { useAnimate } from "motion/react-mini"
```

```javascript
// Hybrid
import { useAnimate } from "motion/react"
```

--------------------------------

### Glide Animation with Value-Specific Options

Source: https://motion.dev/docs/glide

Demonstrates how to apply different easing functions and velocities to individual animated properties. In this example, the x-axis uses glide with 200 units/second velocity while the y-axis uses spring with 500 units/second velocity.

```javascript
animate(
  "#ball",
  { x: 0, y: 0 },
  {
    x: { easing: glide({ velocity: 200 }) },
    y: { easing: spring({ velocity: 500 }) }
  }
)
```

--------------------------------

### Motion component initial prop with animation target

Source: https://motion.dev/docs/react-motion-component

Set the initial visual state of a motion component using an animation target object. This defines the starting state before any animations are applied. The initial prop can accept animation targets, variants, or be set to false to disable enter animations.

```javascript
<motion.section initial={{ opacity: 0, x: 0 }} />
```

--------------------------------

### SDK Function: fromShareURL

Source: https://motion.dev/docs/studio-sdk-state

Parses a `TransitionState` object from a full URL string's query parameters. Returns `null` if the `transition` parameter is missing or invalid.

```APIDOC
## fromShareURL

### Description
Parses a new `TransitionState` out of a full URL string. Returns `null` if the `transition` parameter is missing or invalid.

### Method
Function Call

### Endpoint
N/A

### Parameters
#### Function Parameters
- **url** (string) - Required - The full URL string to parse.

### Request Example
```json
"https://example.com/?transition=%7B%22type%22%3A%22spring%22%2C%22easing%22%3A%7B%22duration%22%3A0.5%2C%22ease%22%3A%5B0.25%2C0.1%2C0.25%2C1%5D%7D%2C%22spring%22%3A%7B%22duration%22%3A0.8%2C%22bounce%22%3A0.2%2C%22stiffness%22%3A100%2C%22damping%22%3A10%2C%22mass%22%3A1%2C%22type%22%3A%22physics%22%2C%22isVisualDuration%22%3Atrue%7D%7D"
```

### Response
#### Success Response (TransitionState | null)
- **state** (TransitionState | null) - The parsed `TransitionState` object, or `null` if the `transition` parameter is missing or invalid.

#### Response Example
```json
{
  "type": "spring",
  "easing": {
    "duration": 0.5,
    "ease": [0.25, 0.1, 0.25, 1]
  },
  "spring": {
    "duration": 0.8,
    "bounce": 0.2,
    "stiffness": 100,
    "damping": 10,
    "mass": 1,
    "type": "physics",
    "isVisualDuration": true
  }
}
```
```

--------------------------------

### Detect hover on DOM element with Motion

Source: https://motion.dev/docs/hover

Attach a hover gesture listener to a specific DOM element using its reference. The callback receives the element and PointerEvent when hover starts.

```javascript
hover(
  document.getElementById("my-id"),
  () => {
    console.log("my-id hovered!")
  }
)
```

--------------------------------

### Implementing `LazyMotion` with `domAnimation` for basic animations in Vue

Source: https://motion.dev/docs/vue-lazymotion

Demonstrates the basic usage of `LazyMotion` in a Vue component. It shows how to import `LazyMotion`, `domAnimation`, and `m`, then wrap an `m.div` component with `LazyMotion` to enable animations using the `domAnimation` feature package.

```javascript
import { LazyMotion, domAnimation, m } from "motion-v"
```

```html
<template>
<!--Load only the domAnimation package-->
<LazyMotion :features="domAnimation">
<m.div :animate="{ opacity: 1 }" />
</LazyMotion>
</template>
```

--------------------------------

### Configure drag distance threshold

Source: https://motion.dev/docs/react-use-drag-controls

Set the minimum cursor travel distance required to initialize a drag gesture using the distanceThreshold option. Default is 3 pixels; this example sets it to 10 pixels.

```javascript
controls.start(event, { distanceThreshold: 10 })
```

--------------------------------

### Style Cursor with className and inline styles

Source: https://motion.dev/docs/cursor

Customize the Cursor component's appearance using CSS className and inline style properties. This example sets a custom class and changes the background color to red.

```jsx
<Cursor className="my-cursor" style={{ backgroundColor: "red" }} />
```

--------------------------------

### Implement Exit Animations for Base UI Components with AnimatePresence (React)

Source: https://motion.dev/docs/base-ui

This section illustrates how to add exit animations to Base UI components using Motion's `AnimatePresence`. It covers the standard approach for components that are conditionally rendered, and then details the specific steps required for components like `ContextMenu` and `Popover` that manage their own conditional rendering. These steps include hoisting the `open` state, using `keepMounted` on the `Portal` component, and wrapping the `Portal` with `AnimatePresence`.

```jsx
<AnimatePresence>
  {open && (
    <Menu.Trigger render={
      <motion.button
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
        exit={{ opacity: 0 }}
      />
    } />
  )}
</AnimatePresence>
```

```jsx
const [open, setOpen] = useState(false)

return (
  <ContextMenu.Root open={open} onOpenChange={setOpen}>

```

```jsx
return (
   <ContextMenu.Root open={open} onOpenChange={setOpen}>
    <ContextMenu.Trigger>Open menu</ContextMenu.Trigger>
    <AnimatePresence>
      {open && (
        <ContextMenu.Portal keepMounted>

```

```jsx
function App() {
  const [open, setOpen] = useState(false)
  
  return (
    <ContextMenu.Root open={open} onOpenChange={setOpen}>
      <ContextMenu.Trigger>Open menu</ContextMenu.Trigger>
      <AnimatePresence>
        {open && (
          <ContextMenu.Portal keepMounted>
            <ContextMenu.Positioner>
              <ContextMenu.Popup
                render={
                  <motion.div
                    initial={{ opacity: 0, transform: "scale(0.9)" }}
                    animate={{ opacity: 1, transform: "scale(1)" }}
                    exit={{ opacity: 0, transform: "scale(0.9)" }}
                  />
                }
              >
                {/* Children */}
              </ContextMenu.Popup>

```

--------------------------------

### Apply Focus Gesture Animation with `whileFocus` in Vue

Source: https://motion.dev/docs/vue-gestures

This example illustrates the use of the `whileFocus` prop on a `motion.a` component. It applies animations (e.g., `scale: 1.2`) when the component gains focus, adhering to the same rules as the CSS `:focus-visible` selector for accessibility.

```html
<motion.a :whileFocus="{ scale: 1.2 }" href="#" />
```

--------------------------------

### Define Animation Sequence with Default Timing

Source: https://motion.dev/docs/animate

Creates a sequence array where animations start sequentially by default. Each animation begins when the previous one completes. This provides a simple way to chain multiple animations together in order.

```javascript
const sequence = [
  ["ul", { opacity: 1 }],
  // This will start when ul opacity is 1
  ["li", { x: [-100, 0] }]
]
```

--------------------------------

### Apply Staggered Delay to ScrambleText in React

Source: https://motion.dev/docs/react-scramble-text

Demonstrates how to use Motion's `stagger` function with the `delay` prop. This causes characters to start scrambling one-by-one, while the overall reveal duration remains consistent for each character.

```jsx
// Chars start scrambling one-by-one, all reveal after 1s of scrambling
<ScrambleText delay={stagger(0.1)} duration={1}>
  Hello world!
</ScrambleText>
```

--------------------------------

### Import Mini Motion Animate Function via CDN

Source: https://motion.dev/docs/webflow

This script imports only the `animate` function from the mini version of the Motion library via CDN. This approach significantly reduces the filesize to 2.3kb, making it ideal for scenarios where only basic animation functionality is required and performance is critical. It should be placed in the 'Before `<body>` tag' section.

```html
<script type="module">
  import { animate } from "https://cdn.jsdelivr.net/npm/motion@11.13.5/mini/+esm"
</script>
```

--------------------------------

### Apply MotionValue to multiple SVG properties and elements (JavaScript)

Source: https://motion.dev/docs/svg-effect

This example highlights the flexibility of `svgEffect`, where a single `motionValue` can be applied to multiple styles or attributes on one or more elements. Here, a `progress` motion value controls both `pathLength` and `pathOffset` for an element with the ID '#progress'.

```JavaScript
const progress = motionValue(0)

svgEffect("#progress", {
  pathLength: progress,
  pathOffset: progress
})
```

--------------------------------

### Import useVelocity Hook (React)

Source: https://motion.dev/docs/react-use-velocity

Shows the standard way to import the `useVelocity` hook from the `motion/react` library, making it available for use within React components to track motion value velocities.

```javascript
import { useVelocity } from "motion/react"
```

--------------------------------

### Tree-shake Motion with bundler for WordPress

Source: https://motion.dev/docs/wordpress

Demonstrates importing only the animate function from Motion and bundling with Rollup for optimal file size. The bundled script is uploaded to a CDN and included with an async tag, improving SEO and performance by eliminating unused library code.

```javascript
import { animate } from "motion"

animate("header", { opacity: 1 })
```

```html
<script async src="https://yourdomain.com/my-script.js"></script>
```

--------------------------------

### whileInView - Animate on Viewport Entry

Source: https://motion.dev/docs/react-motion-component

Triggers animations when an element enters the viewport. Accepts either target values or variant names. Useful for scroll-triggered animations without manual intersection observer setup.

```jsx
<motion.div whileInView={{ opacity: 1 }} />
```

```jsx
<motion.div whileInView="visible" />
```

--------------------------------

### Predefined Character Sets for scrambleText

Source: https://motion.dev/docs/scramble-text

Provides examples of predefined character sets that can be used with the `chars` option in `scrambleText`. These constants offer quick access to common character types like symbols, blocks, binary, hex, Katakana, and dots for various animation styles.

```javascript
const symbols = "!@#$%^&*()_+-=[]{}|;:,.<>?/~`░▒▓█▀▄■□▪▫●○◆◇◈◊※†‡"
const blocks = "█▓▒░"
const binary = "01"
const hex = "0123456789ABCDEF"
const katakana = "アイウエオカキクケコサシスセソタチツテトナニヌネノハヒフヘホマミムメモヤユヨラリルレロワヲン"
const dots = "⠁⠂⠃⠄⠅⠆⠇⠈⠉⠊⠋⠌⠍⠎⠏"
```

--------------------------------

### Replace deprecated exitBeforeEnter prop in Framer Motion 10.0

Source: https://motion.dev/docs/react-upgrade-guide

The exitBeforeEnter prop on AnimatePresence was deprecated in version 7.2.0 and now throws an error in version 10.0. Replace it with the mode="wait" prop.

```javascript
// Old (deprecated)
<AnimatePresence exitBeforeEnter>
  {/* content */}
</AnimatePresence>

// New
<AnimatePresence mode="wait">
  {/* content */}
</AnimatePresence>
```

--------------------------------

### Importing inView Function (JavaScript)

Source: https://motion.dev/docs/inview

Illustrates the standard way to import the `inView` function from the `motion` library into a JavaScript file, making it available for use.

```javascript
import { inView } from "motion"
```

--------------------------------

### Create Infinite ScrambleText on Hover in React

Source: https://motion.dev/docs/react-scramble-text

Provides a functional React component example demonstrating an infinite scrambling effect that activates when the user hovers over the text. It utilizes React's `useState` hook to manage the `active` prop and sets `duration` to `Infinity`.

```jsx
function HoverScrambleEffect() {
  const [isHovered, setIsHovered] = useState(false)

  return (
    <ScrambleText
      active={isHovered}
      duration={Infinity}
      onMouseEnter={() => setIsHovered(true)}
      onMouseLeave={() => setIsHovered(false)}
    >
      Hover me!
    </ScrambleText>
  )
}
```

--------------------------------

### Applying `scope` Ref to a React Element

Source: https://motion.dev/docs/react-use-animate

To define the scope for animations, the `scope` ref returned by `useAnimate` must be attached to a DOM element or a `motion` component. This example demonstrates attaching the `scope` ref to an `<ul>` element, making it the root for all subsequent scoped animations.

```javascript
function Component({ children }) {
  const [scope, animate] = useAnimate()
  
  return <ul ref={scope}>{children}</ul>
}
```

--------------------------------

### Import attrEffect from Motion

Source: https://motion.dev/docs/attr-effect

Shows the import statement required to use attrEffect in your project. This must be done before calling the attrEffect function.

```javascript
import { attrEffect } from "motion"
```

--------------------------------

### Animating Scoped Children with a CSS Selector using `useAnimate`

Source: https://motion.dev/docs/react-use-animate

This example demonstrates using a CSS selector with the `animate` function to target specific child elements within the scoped container. The `animate` function automatically restricts the selector to only children of the element with the `scope` ref, preventing global selections.

```javascript
animate("li", { backgroundColor: "#000" }, { ease: "linear" })
```

--------------------------------

### Customize dragTransition inertia animation properties

Source: https://motion.dev/docs/vue-motion-component

Modify the dragging momentum transition by customizing the inertia animation that starts when a draggable element is released. Allows adjustment of bounceStiffness, bounceDamping, and other animation parameters based on dragging velocity.

```vue
<motion.div
  drag
  :dragTransition="{ bounceStiffness: 600, bounceDamping: 10 }"
/>
```

--------------------------------

### Update event handlers from mouse/touch to pointer events in Framer Motion 8.0

Source: https://motion.dev/docs/react-upgrade-guide

Framer Motion 8.0 removes polyfills for mouse and touch events. DragControls.start now only accepts onPointerDown events. Update onMouseDown and onTouchStart handlers to use onPointerDown.

```javascript
// Old (no longer works)
const controls = useDragControls()

const handleMouseDown = (event) => {
  controls.start(event) // Type error in TypeScript
}

// New
const controls = useDragControls()

const handlePointerDown = (event) => {
  controls.start(event)
}

<div onPointerDown={handlePointerDown}>
  Draggable content
</div>
```

--------------------------------

### Importing `m` component for bundle size optimization in JavaScript

Source: https://motion.dev/docs/vue-lazymotion

Explains how to import the lightweight `m` component from `motion-v` as an alternative to the full `motion` component, reducing initial bundle size. This component is used with `LazyMotion` to selectively load features.

```javascript
import { m } from "motion-v"
```

--------------------------------

### Control ScrambleText Playback with Active Prop in React

Source: https://motion.dev/docs/react-scramble-text

Demonstrates how to dynamically start and stop the `ScrambleText` animation by toggling a boolean value passed to the `active` prop. When `active` becomes false, any ongoing scrambling immediately resolves to the final text.

```jsx
<ScrambleText active={active} duration={1}>
  Hello world!
</ScrambleText>
```

--------------------------------

### Disable automatic drag listener on motion component

Source: https://motion.dev/docs/react-use-drag-controls

Prevent automatic drag gesture initiation on the motion component itself by setting dragListener={false} prop. This allows exclusive control through the drag controls start method.

```javascript
<motion.div
  drag
  dragListener={false}
  dragControls={controls}
/>
```

--------------------------------

### Using the wrap function for cyclic range management in JavaScript

Source: https://motion.dev/docs/wrap

Demonstrates the `wrap` function's behavior for constraining values within a cyclic range. It illustrates cases where the value is within the range (returned unchanged), above the maximum (wrapped to the beginning), and below the minimum (wrapped to the end), useful for scenarios like pagination or circular arrays.

```javascript
wrap(0, 100, 150) // 50
```

```javascript
const index = wrap(0, numItems, currentIndex + 1)
```

```javascript
wrap(0, 10, 5) // 5
```

```javascript
wrap(0, 10, 11) // 1
wrap(0, 10, -1) // 9
```

--------------------------------

### Transform Motion Value with useTransform Hook

Source: https://motion.dev/docs/react-motion-value

Shows how to create a derived motion value using useTransform that maps input values from one motion value to output values. In this example, the opacity changes as an element is dragged left and right based on the x position.

```jsx
const x = useMotionValue(0)
const opacity = useTransform(
  x,
  [-200, 0, 200],
  [0, 1, 0]
)

// Will change opacity as element is dragged left/right
return <motion.div drag="x" style={{ x, opacity }} />
```

--------------------------------

### Set Spring Animation Visual Duration in Motion (Vue)

Source: https://motion.dev/docs/vue-transitions

This example explains how to use `visualDuration` to control the perceived duration of a spring animation, overriding the standard `duration` property. It allows you to specify a time in seconds for the animation to visually appear to reach its target, making it easier to coordinate with other time-based animations.

```vue
<motion.div
  :animate="{ rotateX: 90 }"
  :transition="{
    type: 'spring',
    visualDuration: 0.5,
    bounce: 0.25
  }"
/>
```

--------------------------------

### Import usePageInView from Motion React

Source: https://motion.dev/docs/react-use-page-in-view

Import the usePageInView hook from the motion/react package to access page visibility tracking functionality.

```javascript
import { usePageInView } from "motion/react"
```

--------------------------------

### Parse TransitionState from URL String in Motion Studio

Source: https://motion.dev/docs/studio-sdk-state

This snippet demonstrates how to use the `fromShareURL` utility to parse a full URL string and reconstruct a `TransitionState` object from its query parameters. It allows loading animation configurations from shared URLs, returning `null` if the 'transition' parameter is missing or invalid.

```typescript
import { fromShareURL } from "motion-studio"

const state = fromShareURL(window.location.href)
```

--------------------------------

### Implement Drag Gesture with `drag` and `whileDrag` in Vue

Source: https://motion.dev/docs/vue-gestures

This example demonstrates enabling dragging on a `motion.div` component using the `drag` prop. It also applies animations during the drag gesture using `whileDrag`, changing `scale` and `backgroundColor` as the element is moved.

```html
<motion.div drag :whileDrag="{ scale: 1.2, backgroundColor: '#f00' }" />
```

--------------------------------

### Set Animation Sequence Timing to Labelled Time

Source: https://motion.dev/docs/animate

Uses the 'at' parameter with a label name to start an animation at the same point as a previously defined label. Labels are defined as strings in the sequence array and enable reusable timing references.

```javascript
const sequence = [
  ["nav", { x: 100 }, { duration: 1 }],
  
  "my-label", // label definition
  ["li", { opacity: 1 }],
  
  // my-label was defined at 1 second
  ["a", { scale: 1.2 }, { at: "my-label" }],
]
```

--------------------------------

### useInView with Amount Option in React

Source: https://motion.dev/docs/react-use-in-view

Demonstrates the amount option to control how much of an element must be visible to be considered in view. Accepts 'some', 'all', or a number between 0 and 1 representing the percentage of the element that must be visible.

```javascript
import { useInView } from "motion/react"
import { useRef } from "react"

function Component() {
  const ref = useRef(null)
  const isInView = useInView(ref, { amount: "all" })
  
  return <div ref={ref} />
}
```

--------------------------------

### Mirror an Easing Function with `mirrorEasing` Modifier

Source: https://motion.dev/docs/easing-functions

This snippet illustrates the use of the `mirrorEasing` modifier to create a new easing function that mirrors an existing one. This can transform an 'easeIn' function into an 'easeIn-Out' effect, providing acceleration at both the start and end of the animation.

```javascript
import { mirrorEasing } from "motion"

const powerIn = (progress) => progress * progress

const powerInOut = mirrorEasing(powerInOut)
```

--------------------------------

### Basic `useTransform` with Value Mapping Placeholders (React)

Source: https://motion.dev/docs/react-use-transform

Shows the general syntax for `useTransform` when using value mapping, where an input motion value is transformed based on defined input and output ranges. `input` and `output` are placeholders for actual arrays.

```javascript
const opacity = useTransform(x, input, output)
```

--------------------------------

### useTransform with Clamp Option

Source: https://motion.dev/docs/vue-use-transform

Demonstrates the clamp option behavior. When clamp is true (default), output is restricted to the range. When false, mapping continues beyond the range limits.

```JavaScript
const y = useTransform(x, [0, 1], [0, 2])
const z = useTransform(x, [0, 1], [0, 2], { clamp: false })

onMounted(() => {
  x.set(2)
  console.log(y.get()) // 2, input clamped
  console.log(z.get()) // 4
})
```

--------------------------------

### Accessing Animation Controls with animate() (JavaScript)

Source: https://motion.dev/docs/animate

The `animate()` function returns an animation object that provides various playback controls. This example demonstrates how to access and use basic controls like setting the current time and stopping the animation.

```javascript
const animation = animate(element, { opacity: 1 })

animation.time = 0.5
animation.stop()
```

--------------------------------

### Fix Layout Animation Distortion with borderRadius in Motion 2

Source: https://motion.dev/docs/react-upgrade-guide

Demonstrates how to prevent `borderRadius` and `boxShadow` distortion during layout animations in Motion 2 by explicitly animating these properties. This fix is applied when components change size during layout animations.

```jsx
<motion.div layout initial={{ borderRadius: 20 }} />
```

--------------------------------

### Apply MotionValue to SVG `cx` attribute with `svgEffect` (JavaScript)

Source: https://motion.dev/docs/svg-effect

This example demonstrates the basic usage of `svgEffect` to link a `motionValue` to an SVG element's attribute. When the `cx` motion value updates, the 'circle' element will automatically re-render, reflecting the new `cx` position.

```JavaScript
const cx = motionValue(100)

svgEffect("circle", { cx })
```

--------------------------------

### Use Motion Values for advanced 3D animations in Framer Motion 3D

Source: https://motion.dev/docs/react-three-fiber

This example demonstrates the use of `useMotionValue` to track an animating value (`x`) and `useTransform` to derive another value (`scaleZ`) from it. These motion values are then applied to a `motion.mesh` component's `position-x` and `scale` attributes, allowing for complex, interdependent animations outside of React's render cycle.

```jsx
import { useMotionValue, useTransform } from "framer-motion"
import { motion } from "framer-motion-3d"

export function Box() {
  const x = useMotionValue(0)
  const scaleZ = useTransform(x, v => v / 100)
  
  return (
    <motion.mesh
      position-x={x}
      scale={[1, 1, scaleZ]}
      animate={{ x: 100 }} 
    />
  )
}
```

--------------------------------

### Configuring inView Margin Option (JavaScript)

Source: https://motion.dev/docs/inview

Demonstrates how to use the `margin` option to extend or contract the viewport boundaries. This allows for triggering detection before an element visually enters or after it leaves the actual viewport, using CSS-like margin values.

```javascript
inView(element, callback, { margin: "0px 100px 0px 0px" })
```

--------------------------------

### Disable automatic drag with dragListener prop

Source: https://motion.dev/docs/vue-use-drag-controls

Set the drag-listener prop to false on the motion component to prevent automatic drag gesture initiation from pointerdown events. This allows exclusive control via the useDragControls start method.

```vue
<template>
  <motion.div
    drag
    :drag-listener="false"
    :drag-controls="controls"
  />
</template>
```

--------------------------------

### Integrate LayoutCamera in React Three Fiber with MotionCanvas

Source: https://motion.dev/docs/react-three-fiber-layout-cameras

This snippet demonstrates how to integrate `LayoutCamera` into a React Three Fiber scene using Framer Motion. It requires replacing the standard `@react-three/fiber` `Canvas` component with `MotionCanvas` and then adding `LayoutCamera` within the scene hierarchy. This setup enables 3D scenes to participate in Motion's layout animations by pre-distorting the camera view.

```javascript
import { MotionCanvas, LayoutCamera } from "framer-motion"

function Scene() {
  <MotionCanvas>
    <LayoutCamera />
    <Box />
  </MotionCanvas>
}
```

--------------------------------

### Importing `useTransform` from Motion (React)

Source: https://motion.dev/docs/react-use-transform

Shows the standard way to import the `useTransform` hook from the `motion/react` library, making it available for use within React components.

```javascript
import { useTransform } from "motion/react"
```

--------------------------------

### Import Motion from motion/react package

Source: https://motion.dev/docs/figma

Shows the recommended import statement for Motion in React projects. This import should be added to the top of your component file to access Motion components and utilities. The motion/react package is the current standard import path for Motion.

```javascript
import { motion } from "motion/react"
```

--------------------------------

### Get Velocity from Motion Value

Source: https://motion.dev/docs/react-motion-value

Shows how to retrieve the velocity of a motion value using getVelocity() method. The velocity is calculated per second to account for frame rate variations across devices. Returns 0 for string and color values.

```javascript
const xVelocity = x.getVelocity()
```

--------------------------------

### Animate Rounded Corners with `clipPath` (More Performant) in JavaScript

Source: https://motion.dev/docs/performance

This JavaScript example illustrates a more performant method for animating rounded corners using the `clipPath` CSS property with the `inset` function. `clipPath` animations are increasingly supported by browsers for hardware acceleration, offering smoother performance than direct `borderRadius` animations.

```javascript
// ✅
animate(element, { clipPath: "inset(0 round 50px)" })
```

--------------------------------

### Disabling Clamping for mapValue Ranges (JavaScript)

Source: https://motion.dev/docs/map-value

This example demonstrates how to disable the default clamping behavior of `mapValue` by passing `{ clamp: false }` as an option. This allows the output value to extrapolate beyond the defined output range based on the input motion value, providing more flexible interpolation.

```javascript
const progress = motionValue(3)
const double = mapValue(progress, [0, 1], [0, 2], { clamp: false })

double.get() // 6
```

--------------------------------

### Import `useMotionTemplate` from Motion (React)

Source: https://motion.dev/docs/react-use-motion-template

This snippet illustrates the standard way to import the `useMotionTemplate` hook from the `motion/react` package, making it available for use within React components that utilize Motion.

```javascript
import { useMotionTemplate } from "motion/react"
```

--------------------------------

### Setup Motion Components with Radix-Vue `asChild` Prop

Source: https://motion.dev/docs/vue-radix

This snippet shows how to integrate a Motion component with a Radix component (e.g., `ToastRoot`) by setting the `asChild` prop to `true`. This allows the Radix component to use the Motion component as its DOM node, enabling Motion's animation props like `initial`, `animate`, and `layout`.

```Vue
<template>
<ToastRoot :as-child="true">
<Motion
:initial="{ opacity: 0 }"
:animate="{ opacity: 1 }"
layout
>

```

--------------------------------

### Initiate drag from external component with useDragControls

Source: https://motion.dev/docs/react-motion-component

Use the useDragControls hook to create drag controls that can be passed to a draggable component. Exposes a start method to initiate dragging from pointer events on other components, useful for custom drag initiators like video scrubbers.

```JSX
const dragControls = useDragControls()

function startDrag(event) {
  dragControls.start(event, { snapToCursor: true })
}

return (
  <>
    <div onPointerDown={startDrag} />
    <motion.div drag="x" dragControls={dragControls} />
  </>
)
```

--------------------------------

### Import Motion.js `animate` for Bundlers (Tree-Shaking)

Source: https://motion.dev/docs/squarespace

This JavaScript snippet shows the syntax for importing the `animate` function from Motion.js when using a module bundler like Vite or Rollup. This approach enables tree-shaking, ensuring that only the necessary parts of the library are included in the final bundle, leading to smaller file sizes and improved performance. This code is intended for local development and bundling, not direct Squarespace injection.

```javascript
import { animate } from "motion"

animate("header", { opacity: 1 })
```

--------------------------------

### Implement LazyMotion for bundle size reduction in Framer Motion 4.0

Source: https://motion.dev/docs/react-upgrade-guide

Use the LazyMotion component with domAnimation features to reduce bundle size by loading only necessary animation functionality. This replaces the deprecated MotionConfig features prop approach from earlier versions.

```javascript
import { LazyMotion, domAnimation, m } from "framer-motion"

export const MyComponent = ({ isVisible }) => (
  <LazyMotion features={domAnimation}>
    <m.div animate={{ opacity: 1 }} />
  </LazyMotion>
)
```

--------------------------------

### Customize `whileHover` animation transitions in React Motion

Source: https://motion.dev/docs/react-hover-animation

This example demonstrates how to customize the transition properties for `whileHover` animations. You can define a specific `transition` object within the `whileHover` prop for the hover-in animation, and a separate `transition` prop on the component for the hover-out animation, allowing fine-grained control over timing.

```jsx
<motion.button
whileHover={{
scale: 1.1,
// Will be used when gesture starts
transition: { duration: 0.1 }
}}
// Will be used when gesture ends
transition={{ duration: 0.5 }}
/>
```

--------------------------------

### Conditionally Animate with Opacity or Transform in React

Source: https://motion.dev/docs/react-accessibility

Provides an example of how to conditionally apply different animation properties (`opacity` vs. `x` or `y` transforms) based on the `shouldReduceMotion` boolean from the `useReducedMotion` hook. This allows for smoother, less jarring transitions for users with reduced motion enabled.

```javascript
function Sidebar({ isOpen }) {
  const shouldReduceMotion = useReducedMotion()
  let animate

  if (isOpen) {
    animate = shouldReduceMotion ? { opacity: 1 } : { x: 0 }
  } else {
    animate = shouldReduceMotion
      ? { opacity: 0 }
      : { x: "-100%" }
  }

  return <motion.div animate={animate} />
}
```

--------------------------------

### Interrupt Animation with WAAPI

Source: https://motion.dev/docs/improvements-to-the-web-animations-api-dx

Demonstrates WAAPI's default behavior when a new animation starts while another is playing on the same value. The new animation overrides the old one, causing the value to jump back if the old animation is still running.

```javascript
element.animate(
  { transform: ["none", "translateX(300px)"] },
  { duration: 2000, iterations: Infinity, direction: "alternate" }
)
  
setTimeout(() => {
  element.animate({ transform: "none" }, { duration: 500 })
}, 500)
```

--------------------------------

### Animate Drop Shadow with `filter` (More Performant) in JavaScript

Source: https://motion.dev/docs/performance

This JavaScript example demonstrates a more performant approach to animating a drop shadow by using the `filter` CSS property with the `drop-shadow` function. Browsers are increasingly capable of hardware-accelerating `filter` animations, leading to smoother results compared to animating `boxShadow` directly.

```javascript
// ✅
animate(element, { filter: "drop-shadow(10px 10px black)" })
```

--------------------------------

### Initiate drag from external component using dragControls

Source: https://motion.dev/docs/vue-motion-component

Use the useDragControls hook to create drag controls that can initiate dragging from a different component than the draggable element. The start method accepts pointer events and options like snapToCursor. Set dragListener to false to disable default drag initiation.

```vue
<script setup>
  const dragControls = useDragControls()
  
  function startDrag(event) {
    dragControls.start(event, { snapToCursor: true })
  }
</script>

<template>
  <div @pointerDown="startDrag" />
  <motion.div drag="x" :dragControls="dragControls" />
</template>
```

--------------------------------

### Track viewport size changes with resize callback

Source: https://motion.dev/docs/resize

Detect viewport changes by passing a callback to resize. The callback receives an object with width and height getters that return the current viewport dimensions.

```JavaScript
resize(() => console.log("viewport change detected"))

// With width and height getters
resize(({ width, height }) => console.log(width, height))
```

--------------------------------

### Manually Manage Motion Value Event Subscriptions with useEffect

Source: https://motion.dev/docs/react-use-motion-value-event

This advanced example shows how to manually subscribe to motion value events using their `on` method within a React `useEffect` hook. It emphasizes the necessity of returning a cleanup function to unsubscribe from events (`unsubX()`, `unsubY()`) when the component unmounts, preventing memory leaks.

```javascript
useEffect(() => {
  const doSomething = () => {}
  
  const unsubX = x.on("change", doSomething)
  const unsubY = y.on("change", doSomething)
  
  return () => {
    unsubX()
    unsubY()
  }
}, [x, y])
```

--------------------------------

### Motion 11.0 Spring Animation Configuration

Source: https://motion.dev/docs/upgrade-guide

Motion 11.0 changes spring animation creation by passing spring to the type option, with spring-related options moved to the animation's options object rather than a separate spring function. This simplifies the API and consolidates animation configuration.

```javascript
import { animate } from "motion/mini"
import { spring } from "motion"

animate(
  element,
  { transform: "translateX(100px)" },
  { type: spring, stiffness: 400 }
)
```

--------------------------------

### Calculate inverse motionValue for nested transformations in JavaScript

Source: https://motion.dev/docs/transform-value

This example illustrates using `transformValue` to compute an inverse value from an existing `motionValue`. It applies the original scale to a parent element and the inverse scale to a child, useful for maintaining relative sizing during transformations.

```javascript
const scale = motionValue(1)
const inverseScale = transformValue(() => 1 / scale.get())

styleEffect(".parent", { scale })
styleEffect(".child", { scale: inverseScale })
```

--------------------------------

### Respond to element resize with Motion frame loop

Source: https://motion.dev/docs/resize

Use the Motion frame loop to batch DOM operations when responding to element size changes, preventing layout thrashing and optimizing performance during re-renders.

```JavaScript
resize(".drawer", (element, { width, height }) => {
  frame.render(() => {
    element.style.height = Math.max(400, height)
  })
})
```

--------------------------------

### Set Animation Sequence Timing Relative to Previous Animation End

Source: https://motion.dev/docs/animate

Uses the 'at' parameter with '+' or '-' prefix to start an animation relative to the end of the previous animation. Positive values delay after the previous animation ends, negative values overlap before it ends.

```javascript
const sequence = [
  ["nav", { opacity: 1 }, { duration: 1 }],
  
  // 0.5 seconds after the previous animation (1.5 secs):
  ["nav", { x: 100 }, { at: "+0.5" }],
  
  // 0.2 seconds before the end of the previous animation:
  ["nav li", { opacity: 1 }, { at: "-0.2" }],
]
```

--------------------------------

### Use LayoutGroup for shared layout animations in Framer Motion 5.0

Source: https://motion.dev/docs/react-upgrade-guide

Replace AnimateSharedLayout with the new LayoutGroup component to group components that affect each other's layout. This approach is more performant as grouped components are measured but not forced to re-render when siblings change.

```javascript
import { LayoutGroup, motion } from "framer-motion"

export function App() {
  return (
    <LayoutGroup>
      <Submenu />
      <Submenu />
    </LayoutGroup>
  )
}

function Submenu({ children }) {
  const [isOpen, setIsOpen] = useState(false)
  
  return (
    <motion.ul
      layout
      style={{ height: isOpen ? "auto" : 40 }}
    >
      {children}
    </motion.ul>
  )
}
```

--------------------------------

### Share state between React DOM and React Three Fiber for animations

Source: https://motion.dev/docs/react-three-fiber

This example demonstrates how to coordinate animations between a standard React DOM component and a React Three Fiber scene by sharing state. The `isHovered` state, managed by a `framer-motion` div, is passed to the 3D scene, allowing a `framer-motion-3d` group to animate based on DOM interactions.

```jsx
// index.js
import { motion } from "framer-motion"
import { Scene } from "./scene"

export function App() {
  const [isHovered, setIsHovered] = useState(false)
  
  return (
    <motion.div
      whileHover={{ scale: 1.2 }}
      onHoverStart={() => setIsHovered(true)}
      onHoverEnd={() => setIsHovered(true)}
    >
      <Scene isHovered={isHovered} />
    </motion.div>
  )
}
```

```jsx
// scene.js
import { Canvas } from "@react-three/fiber"
import { motion } from "framer-motion-3d"

export function Scene({ isHovered }) {
  return (
    <Canvas>
      <motion.group animate={isHovered ? "hover" : "rest"}>
        <motion.mesh variants={{ hover: { z: 1 } }} />
      </motion.group>
    </Canvas>
  )
}
```

--------------------------------

### Comparing `useTransform` Function and Value Mapping (React)

Source: https://motion.dev/docs/react-use-transform

Illustrates the two main patterns for using `useTransform`: a direct transform function for dynamic calculations and value mapping for converting one range to another. This snippet provides a quick comparison of both approaches.

```javascript
// Transform function
const doubledX = useTransform(() => x.get() * 2)

// Value mapping
const color = useTransform(x, [0, 100], ["#f00", "00f"])
```

--------------------------------

### Import `delay` from Motion

Source: https://motion.dev/docs/delay

This snippet demonstrates the standard way to import the `delay` function from the Motion library, making it available for use in your JavaScript code.

```javascript
import { delay } from "motion"
```

--------------------------------

### Basic attrEffect Usage with Motion Values

Source: https://motion.dev/docs/attr-effect

Demonstrates basic usage of attrEffect to apply a motion value to an element attribute. The motion value is created with an initial value and passed to attrEffect with a CSS selector and attribute mapping.

```javascript
const width = motionValue(100)

attrEffect("rect", { width })
```

--------------------------------

### Mapping Motion Values to Complex String Formats (JavaScript)

Source: https://motion.dev/docs/map-value

This example illustrates `mapValue`'s capability to map a numerical motion value to complex string formats, such as CSS `box-shadow` properties. It emphasizes the requirement for consistent string structure across the output range, ensuring smooth interpolation between different string states.

```javascript
const boxShadow = mapValue(
  progress,
  [0, 1],
  ["0px 0px 0px rgba(0, 0, 0, 0)", "10px 10px 5px rgba(0, 0, 0, 0.3)"]
)
```

--------------------------------

### Create a Framer Override with Motion Animation in React

Source: https://motion.dev/docs/framer

This React code defines a higher-order component (HOC) that wraps an existing component, applying a rotation animation using Framer Motion's `animate` and `transition` props. It demonstrates how to use the full `motion` component API within Framer overrides, including prop spreading and style merging for custom animations.

```javascript
export function withRotateAnimation(Component): ComponentType {
    return forwardRef((props, ref) => {
        return (
            <Component
                ref={ref}
                {...props}
                animate={{ rotate: 90 }}
                transition={{ duration: 2 }}
                style={{ ...props.style, x: 100 }}
            />
        )
    })
}
```

--------------------------------

### Function: press

Source: https://motion.dev/docs/press

The `press` function detects press gestures, firing events when they start, end, or cancel. It automatically filters out secondary pointer events (like right clicks or a second touch point) and provides keyboard accessibility.

```APIDOC
## Function: press

### Description
Motion's `press` function detects press gestures, firing events when they start, end or cancel. It automatically filters out secondary pointer events and provides keyboard accessibility.

### Type
JavaScript Utility Function

### Import
```javascript
import { press } from "motion"
```

### Parameters
- **target** (string | Element | Element[]) - Required - The element(s) or CSS selector to attach the press listener to.
- **onPressStart** (function) - Required - A callback function that fires when a press gesture starts. It receives `(element, startEvent)` as arguments. This function can optionally return another function to handle the press end.
- **options** (object) - Optional - Configuration options for the press gesture.
    - **`options.passive`** (boolean) - Default: `true` - If `false`, `event.preventDefault()` can be called, but performance may be reduced.
    - **`options.once`** (boolean) - Default: `false` - If `true`, each provided element will fire its gesture only once.

### Callbacks
#### `onPressStart` Callback Signature
```javascript
(element: Element, startEvent: PointerEvent) => (() => (endEvent: PointerEvent, info: { success: boolean }) => void) | void
```
- **`element`** (Element) - The DOM element on which the press started.
- **`startEvent`** (PointerEvent) - The `PointerEvent` that triggered the press start.
- **Returns**: An optional function that will be called when the press gesture ends or is cancelled.

#### `onPressEnd` Callback Signature (returned from `onPressStart`)
```javascript
(endEvent: PointerEvent, info: { success: boolean }) => void
```
- **`endEvent`** (PointerEvent) - The `PointerEvent` that triggered the press end.
- **`info`** (object) - Additional information about the press end.
    - **`info.success`** (boolean) - `true` if the press was successfully completed (like a click), `false` if it ended outside the element or was cancelled (e.g., keyboard blur).

### Returns
- **cancelPress** (function) - A function that, when called, will cancel all active event handlers associated with the gesture.

### Usage Examples
#### Basic Press Detection
```javascript
press("button", (element) => {
  console.log("press started on", element)

  return () => console.log("press ended")
})
```

#### Press with Animation
```javascript
press("button", (element) => {
  animate(element, { scale: 0.9 })

  return () => animate(element, { scale: 1 })
})
```

#### Detecting Press Start on Element
```javascript
press(
  document.getElementById("my-id"),
  () => {
    console.log("my-id pressed!")
  }
)
```

#### Detecting Press Start on CSS Selector
```javascript
press("a", () => console.log("link pressed"))
```

#### Accessing Event Details
```javascript
press("div:nth-child(2)", (element, startEvent) => {
  console.log("Pressed", element)
  console.log("At", startEvent.clientX, startEvent.clientY)
})
```

#### Handling Press End with Success Info
```javascript
press(element, () => {
  return (endEvent, info) => {
    console.log("press ", info.success ? "end" : "cancel")
  }
})
```

#### Cancelling a Press Gesture
```javascript
const cancelPress = press(element, callback)

cancelPress()
```
```

--------------------------------

### Exporting `domAnimation` features for dynamic import in JavaScript

Source: https://motion.dev/docs/vue-lazymotion

Shows how to create a dedicated JavaScript file (`features.js`) that exports the desired `domAnimation` feature package. This file will be dynamically imported later to achieve asynchronous loading, reducing the initial bundle size.

```javascript
// features.js
import { domAnimation } from "motion-v"
export default domAnimation
```

--------------------------------

### Importing useSpring from Motion library

Source: https://motion.dev/docs/vue-use-spring

This snippet demonstrates the standard way to import the `useSpring` hook from the `motion-v` library, making it available for use in your JavaScript or TypeScript components.

```javascript
import { useSpring } from "motion-v"
```

--------------------------------

### Stagger Child Animation Delays with stagger Function

Source: https://motion.dev/docs/vue-transitions

The 'stagger' function creates incremental delays across child animations. By default, stagger applies delays from first to last child. This example staggers delays by 0.1 seconds between each child animation, creating a cascading effect.

```javascript
const transition = {
  delayChildren: stagger(0.1)
}
```

--------------------------------

### Basic LazyMotion Usage with domAnimation (React)

Source: https://motion.dev/docs/react-lazy-motion

This snippet demonstrates the fundamental usage of `LazyMotion` with `domAnimation` to reduce the initial bundle size. It shows how to import `LazyMotion` and the `m` component, then wrap an `m.div` with `LazyMotion` to apply animations efficiently.

```jsx
import { LazyMotion, domAnimation } from "motion/react"
import * as m from "motion/react-m"
  

export const MyComponent = ({ isVisible }) => (
<LazyMotion features={domAnimation}>
<m.div animate={{ opacity: 1 }} />
</LazyMotion>
)
```

--------------------------------

### Generate CSS linear() easing function from Motion spring

Source: https://motion.dev/docs/studio-generate-css

Example of a CSS linear() easing function generated from Motion spring parameters. This represents a spring animation with bounce effect that appears to take 500ms to reach target value. The linear() function contains multiple control points to simulate spring oscillation and is used directly in CSS animations without requiring an animation library.

```css
500ms linear(0, 0.009, 0.035 2.1%, /* ... */)
```

--------------------------------

### Define Animation Priority Order in Motion 3

Source: https://motion.dev/docs/react-upgrade-guide

Establishes the priority ranking for animation states in Motion 3, where animation props are evaluated left-to-right from lowest to highest priority. This determines which animation state takes precedence when multiple props are active simultaneously.

```javascript
const priority = ["animate", "while-", "exit"]
```

--------------------------------

### Optimize `borderRadius` Animation with `will-change` in JavaScript

Source: https://motion.dev/docs/performance

This JavaScript example shows how to use the `will-change` CSS property to hint to the browser that an element's `transform` property will be animated. This can encourage the browser to promote the element to its own graphical layer, potentially improving the performance of subsequent animations like `borderRadius`, which usually trigger a paint.

```javascript
element.style.willChange = "transform"
animate(element, { borderRadius: "50%" })
```

--------------------------------

### Motion 11.0 Animate Callback Function Replacement

Source: https://motion.dev/docs/upgrade-guide

Motion 11.0 replaces the callback function syntax of animate() with the hybrid animate's ability to animate single values, motion values, and objects. The onUpdate callback receives progress values during animation execution.

```javascript
import { animate } from "motion"

animate(0, 1, { onUpdate: (progress) => {} })
```

--------------------------------

### Handle hover start and end events with `onHoverStart` and `onHoverEnd` in React Motion

Source: https://motion.dev/docs/react-hover-animation

Motion components offer `onHoverStart` and `onHoverEnd` event handlers, which fire only on devices truly capable of hover, explicitly filtering out touch-based events. These events allow you to execute custom logic, such as logging, when a hover gesture begins or concludes, providing more control than declarative animations.

```jsx
<motion.a
  onHoverStart={() => console.log('Hover starts')}
  onHoverEnd={() => console.log('Hover ends')}
/>
```

--------------------------------

### Enable Drag Direction Locking with `@directionLock` in Vue

Source: https://motion.dev/docs/vue-gestures

This snippet shows how to enable `dragDirectionLock` on a `motion.div` component. This feature restricts dragging to the first detected axis of movement (horizontal or vertical) after the gesture starts. It also demonstrates using the `@directionLock` event callback.

```html
<motion.div
  drag
  dragDirectionLock
  @directionLock="callback"
/>
```

--------------------------------

### Importing useVelocity Composable

Source: https://motion.dev/docs/vue-use-velocity

This snippet shows the standard JavaScript import statement for the `useVelocity` composable. It is essential to include this line at the top of any script where `useVelocity` will be utilized from the `motion-v` library.

```javascript
import { useVelocity } from "motion-v"
```

--------------------------------

### Basic Typewriter Component Usage in React

Source: https://motion.dev/docs/react-typewriter

Demonstrates the simplest way to use the `Typewriter` component by passing a string as its child. The component will animate the text character by character, emulating a human typing experience.

```jsx
<Typewriter>Hello world!</Typewriter>
```

--------------------------------

### Delay Child Animations with 'delayChildren' Property in Motion Vue

Source: https://motion.dev/docs/vue-transitions

The 'delayChildren' property delays all child animations by a specified duration in seconds. This example shows a container that fades in with a 0.5 second delay before child list items begin their animations. Useful for creating sequential animation effects.

```vue
<script setup>
const container = {
  hidden: { opacity: 0 },
  show: {
    opacity: 1,
    transition: {
      delayChildren: 0.5
    }
  }
}

const item = {
  hidden: { opacity: 0 },
  show: { opacity: 1 }
}
</script>

<template>
  <motion.ul
    :variants="container"
    initial="hidden"
    animate="show"
  >
    <motion.li :variants="item" />
    <motion.li :variants="item"/>
  </motion.ul>
</template>
```

--------------------------------

### Namespace layoutId with LayoutGroup id prop in Framer Motion 5.0

Source: https://motion.dev/docs/react-upgrade-guide

Use the id prop on LayoutGroup to namespace layoutIds and prevent unintended animations between components in different layout groups. This restores the scoping behavior from AnimateSharedLayout while maintaining global batching benefits.

```javascript
/**
 * These layoutIds are now namespaced with
 * the id provided to LayoutGroup.
 */
<>
  <LayoutGroup id="a">
    {isVisible ? <motion.div layoutId="modal" /> : null}
  </LayoutGroup>
  <LayoutGroup id="b">
   {isVisible ? <motion.div layoutId="modal" /> : null}
  </LayoutGroup>
</>
```

--------------------------------

### Correct Child Component Scale Distortion in Motion 2 Layout

Source: https://motion.dev/docs/react-upgrade-guide

Shows how to prevent child component distortion during parent layout animations in Motion 2 by applying the `layout` prop to immediate children. Only direct children require this correction for proper scale handling.

```jsx
<motion.div layout>
  <motion.div layout />
</motion.div>
```

--------------------------------

### Handle keyboard accessibility for tap events in Framer Motion 9.0

Source: https://motion.dev/docs/react-upgrade-guide

Framer Motion 9.0 makes tap events keyboard-accessible by automatically adding tabindex="0" to elements with tap listeners or whileTap. Use tabIndex={-1} to revert this behavior if needed.

```javascript
// Elements with tap listeners automatically receive tabindex="0"
<motion.button whileTap={{ scale: 0.95 }}>
  Click me
</motion.button>

// To revert keyboard accessibility
<motion.button whileTap={{ scale: 0.95 }} tabIndex={-1}>
  Click me
</motion.button>
```

--------------------------------

### Configure Animation Timing with 'when' Property in Motion Vue

Source: https://motion.dev/docs/vue-transitions

The 'when' property controls the orchestration of parent and child animations. Set to 'beforeChildren' to play child animations after the parent, or 'afterChildren' to play parent animations after children finish. This example demonstrates a list with hidden state where children animations complete before the parent animation.

```vue
<script setup>
const list = {
  hidden: {
    opacity: 0,
    transition: { when: "afterChildren" }
  }
}

const item = {
  hidden: {
    opacity: 0,
    transition: { duration: 2 }
  }
}
</script>

<template>
  <motion.ul :variants="list" animate="hidden">
    <motion.li :variants="item" />
    <motion.li :variants="item" />
  </motion.ul>
</template>
```

--------------------------------

### Using inView with Selectors and Elements (JavaScript)

Source: https://motion.dev/docs/inview

Shows the flexibility of `inView` in accepting different target types: a CSS selector string to match multiple elements, or a direct DOM `Element` reference for a single target.

```javascript
// Selector
inView("section", callback)

// Element
const box = document.getElementById("box")
inView(box, callback)
```

--------------------------------

### Import `frame` from Motion

Source: https://motion.dev/docs/frame

This snippet shows how to import the `frame` utility from the Motion library, making it available for use in your JavaScript code.

```javascript
import { frame } from "motion"
```

--------------------------------

### Integrate Motion with Base UI Components using render prop (React)

Source: https://motion.dev/docs/base-ui

This snippet demonstrates how to replace the default DOM element of a Base UI component with a `motion` component using the `render` prop. This allows applying Motion's animation properties like `initial`, `animate`, and `whilePress` directly to the Base UI component's underlying element. It requires importing `Menu` from `@base-ui-components/react/menu` and `motion` from `motion/react`.

```jsx
import { Menu } from "@base-ui-components/react/menu"
import { motion } from "motion/react"

function Component() {
  return (
    <Menu.Trigger render={
      <motion.button
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
        whilePress={{ scale: 0.9 }}
      />
    } />
  )
}
```

--------------------------------

### Apply simple hover animation with `whileHover` prop in React Motion

Source: https://motion.dev/docs/react-hover-animation

The `whileHover` prop provides a declarative way to define a target animation state for a Motion component. When a hover gesture starts, the component animates to the specified values, and reverts to its previous state when the gesture ends. This is the simplest and most common method for adding hover animations.

```jsx
<motion.button whileHover={{ scale: 1.1 }} />
```

--------------------------------

### resize - Element Monitoring

Source: https://motion.dev/docs/resize

Monitor size changes on specific HTML or SVG elements by passing a CSS selector or element reference along with a callback. The callback receives the element and an object with width and height getters.

```APIDOC
## resize(selector, callback)

### Description
Monitor and react to size changes on specific HTML or SVG elements using a CSS selector or element reference.

### Method
Function

### Signature
```javascript
resize(selector: string | Element, callback: (element: Element, dimensions: { width: number, height: number }) => void): () => void
```

### Parameters
#### Selector
- **selector** (string | Element) - Required - CSS selector string or DOM element reference to monitor.

#### Callback Function
- **callback** (function) - Required - Function invoked when element size changes. Receives the element and an object with width and height getters.

### Request Example
```javascript
import { resize } from "motion"

// Monitor specific element by selector
resize("li", (element) => console.log(element, "change detected"))

// Access dimensions
resize(".drawer", (element, { width, height }) => {
  console.log(element, " is now ", width, height)
})

// Respond to size changes with Motion frameloop
resize(".drawer", (element, { width, height }) => {
  frame.render(() => {
    element.style.height = Math.max(400, height)
  })
})
```

### Response
#### Return Value
- **stop** (function) - A cleanup function that removes the listener from the element when called.

### Response Example
```javascript
const stop = resize(".drawer", (element, { width, height }) => {
  console.log("Element size:", width, height)
})

// Later, remove the listener
stop()
```

### Notes
- Width and height represent the element's border box (size including border).
- When there are no more listeners on an element, it is removed from the ResizeObserver.
- When there are no more listeners at all, the ResizeObserver is stopped.
- For best performance, use Motion's frame.render() to batch DOM operations.
```

--------------------------------

### Motion 11.0 Mini Animate Function with Default Values

Source: https://motion.dev/docs/upgrade-guide

Motion 11.0 introduces a mini animate function (2.5kb) that supports default value types and is broadly similar to the old Motion One animate function. The mini version is optimized for small file size but lacks timeline sequencing and independent transform animation capabilities.

```javascript
import { animate } from "motion/mini"

animate(element, { width: 200 })
```

--------------------------------

### Import propEffect from Motion Library

Source: https://motion.dev/docs/prop-effect

Import the propEffect function from the motion package to enable property effect functionality in your project.

```javascript
import { propEffect } from "motion"
```

--------------------------------

### Animate elements with class selector

Source: https://motion.dev/docs/wordpress

Animates elements selected by CSS class using Motion's animate function. This example rotates elements with the 'my-class' class from 0 to 20 to 0 degrees over 0.4 seconds. Classes can be applied via WordPress theme customizer.

```javascript
animate(".my-class", { rotate: [0, 20, 0] }, { duration: 0.4 })
```

--------------------------------

### Update Jest tests for render scheduling changes in Framer Motion 11.0

Source: https://motion.dev/docs/react-upgrade-guide

Motion component renders are now scheduled as microtasks instead of synchronous operations. Jest tests that expect synchronous style updates must be updated to await the next animation frame using the nextFrame utility.

```javascript
render(
  <motion.div
    initial={{ opacity: 0 }}
    animate={{ opacity: 1 }}
    transition={{ false }}
  />
)

await nextFrame()

expect(element).toHaveStyle("opacity: 1")
```

```javascript
// utils.js
import { frame } from "framer-motion"

export async function nextFrame() {
    return new Promise<void>((resolve) => {
        frame.postRender(() => resolve())
    })
}
```

--------------------------------

### onDragStart

Source: https://motion.dev/docs/react-motion-component

Callback function that fires when a drag gesture begins.

```APIDOC
## onDragStart

### Description
Callback function that fires when a drag gesture starts. Provided the triggering `PointerEvent` and `info` object.

### Type
`(event: PointerEvent, info: PanInfo) => void`

### Parameters
- **event** (PointerEvent) - The original DOM `PointerEvent` that triggered the drag start.
- **info** (PanInfo) - An object containing drag-related information at the start of the drag.

### Usage Example
```jsx
<motion.div drag onDragStart={(event, info) => console.log(info.delta.x)} />
```
```

--------------------------------

### Chain useVelocity for Acceleration (React)

Source: https://motion.dev/docs/react-use-velocity

Demonstrates how `useVelocity` can be applied to an existing velocity motion value to derive an acceleration motion value. This chaining pattern allows for tracking higher-order derivatives of motion, such as the rate of change of velocity.

```javascript
const x = useMotionValue(0)
const xVelocity = useVelocity(x)
const xAcceleration = useVelocity(xVelocity)
```

--------------------------------

### Motion 12.0 Gesture Callbacks - press, hover, inView

Source: https://motion.dev/docs/upgrade-guide

Motion 12.0 changes gesture callback signatures to include the element performing the gesture as the first argument. This replaces the previous approach of extracting element identity from event properties. The change applies to press, hover, and inView gestures, providing a canonical and stable reference to the matched element.

```javascript
press("a", (element, startEvent) => {
  return (endEvent) => {}
})

hover("li", (element, startEvent) => {
  return (endEvent) => {}
})

inView("section", (element, startEntry) => {
  return (endEntry) => {}
})
```

--------------------------------

### Executing Callback on Element Entry (JavaScript)

Source: https://motion.dev/docs/inview

Explains that the primary callback function provided to `inView` will execute by default only once, when the target element first enters the viewport. This is ideal for one-time initialization or animation triggers.

```javascript
inView(element, () => {
  console.log("Element has entered the viewport")
})
```

--------------------------------

### useAnimationFrame Basic Usage - Vue

Source: https://motion.dev/docs/vue-use-animation-frame

Basic example of using useAnimationFrame to rotate a DOM element continuously. The callback receives the total elapsed time since initialization, which is used to update the CSS transform property. This creates a smooth rotation effect synchronized with the browser's animation frame rate.

```javascript
useAnimationFrame((time) => {
  domRef.value.style.transform = `rotateY(${time}deg)`
})
```

--------------------------------

### useTransform with Easing Functions

Source: https://motion.dev/docs/vue-use-transform

Applies easing functions to smooth the mixing between output values. Accepts single easing function or array of functions for different segments. Easing functions must be JavaScript functions.

```JavaScript
import { cubicBezier, circOut, useTransform } from 'motion-v'

const y = useTransform(x, [0, 1], [0, 2], { ease: circOut })

const z = useTransform(
  x,
  [0, 1],
  [0, 2],
  { ease: cubicBezier(0.17, 0.67, 0.83, 0.67) }
)
```

--------------------------------

### MotionValue velocity calculation in Framer Motion 11.0

Source: https://motion.dev/docs/react-upgrade-guide

Demonstrates the breaking change in velocity calculations for MotionValue in version 11.0. Multiple synchronous updates within the same animation frame now calculate velocity based on the latest value and the previous frame's value, not intermediate values.

```javascript
const x = motionValue(0)

requestAnimationFrame(() => {
  x.set(100)
  x.getVelocity() // Velocity of 0 -> 100
  x.set(200)
  x.getVelocity() // Velocity of 0 -> 200 (changed from 100 -> 200)
})
```

--------------------------------

### Optimize Framer Motion Animation with CSS Transform

Source: https://motion.dev/docs/animation-performance-audit

This improved React component demonstrates how to optimize the previous animation. By combining 'scale' and 'rotate' into a single 'transform' property, the animation can run entirely on the GPU, significantly improving performance. This is an example of a recommendation provided by the Animation Performance Audit to achieve better performance.

```jsx
<motion.div
  animate={{
    transform: [
      "scale(1) rotate(0deg)",
      "scale(2) rotate(0deg)",
      "scale(2) rotate(180deg)",
      "scale(2) rotate(180deg)",
      "scale(1) rotate(0deg)"
    ],
    borderRadius: ["0%", "0%", "50%", "50%", "0%"],
  }}
  transition={{ repeat: Infinity }}
/>
```

--------------------------------

### Import styleEffect from Motion

Source: https://motion.dev/docs/style-effect

Import the styleEffect function from the Motion library to enable dynamic style binding to motion values.

```javascript
import { styleEffect } from "motion"
```

--------------------------------

### Motion 11.0 Hybrid Animate Function with Transforms

Source: https://motion.dev/docs/upgrade-guide

Motion 11.0 hybrid animate function (18kb) supports timeline sequencing and independent transform animation. Required for advanced animation features that the mini version does not provide. The hybrid version uses optimized transform string building for better performance than CSS variable approaches.

```javascript
import { animate } from "motion"

animate(element, { x: 100 })
```

--------------------------------

### Track Radix Tooltip state for exit animations

Source: https://motion.dev/docs/radix

Demonstrates how to use Radix Tooltip's open and onOpenChange props to externally manage tooltip state, enabling conditional rendering and exit animations through AnimatePresence.

```jsx
const [isOpen, setOpen] = useState(false)

return (
  <Tooltip.Provider>
    <Tooltip.Root open={isOpen} onOpenChange={setOpen}>
      <AnimatePresence>
        {isOpen && (
          <Tooltip.Portal forceMount>
            <Tooltip.Content asChild>
              <motion.div
                exit={{ opacity: 0 }}
              />
            </Tooltip.Content>
          </Tooltip.Portal>
        )}
      </AnimatePresence>
    </Tooltip.Root>
  </Tooltip.Provider>
)
```

--------------------------------

### Vue Component with Drop Shadow Motion Template

Source: https://motion.dev/docs/vue-use-motion-template

Shows useMotionTemplate with spring animation values for creating a dynamic drop-shadow filter. The shadow position updates smoothly based on spring motion values.

```vue
<script setup>
const shadowX = useSpring(0)
const shadowY = useMotionValue(0)
const filter = useMotionTemplate`drop-shadow(${shadowX}px ${shadowY}px 20px rgba(0,0,0,0.3))`
</script>

<template>
<motion.div :style="{ filter }" />
</template>
```

--------------------------------

### Create dynamic `drop-shadow` with `useSpring` and `useMotionValue` (React)

Source: https://motion.dev/docs/react-use-motion-template

This snippet demonstrates `useMotionTemplate`'s versatility in integrating different types of motion values, specifically `useSpring` (`shadowX`) and `useMotionValue` (`shadowY`), to create a dynamic `drop-shadow` CSS property. The `filter` motion value updates in real-time as `shadowX` and `shadowY` change, applying the visual effect to a `motion.div`.

```javascript
const shadowX = useSpring(0)
const shadowY = useMotionValue(0)

const filter = useMotionTemplate`drop-shadow(${shadowX}px ${shadowY}px 20px rgba(0,0,0,0.3))`

return <motion.div style={{ filter }} />
```

--------------------------------

### Import useMotionTemplate from Motion

Source: https://motion.dev/docs/vue-use-motion-template

Import the useMotionTemplate composable from the motion-v library. This is required before using the tagged template function in Vue components.

```javascript
import { useMotionTemplate } from "motion-v"
```

--------------------------------

### Define TransitionState and Configuration Types in Motion Studio

Source: https://motion.dev/docs/studio-sdk-state

This code defines the TypeScript interfaces for `TransitionType`, `EasingConfig`, `SpringConfig`, and `TransitionState`. These types specify the structure and properties required for configuring animation transitions, including duration, easing functions, and various spring physics parameters.

```typescript
type TransitionType = "easing" | "spring"

interface EasingConfig {
  duration: number
  ease: BezierDefinition
}

interface SpringConfig {
  duration: number
  bounce: number
  stiffness: number
  damping: number
  mass: number
  type: "time" | "physics"
  isVisualDuration: boolean
}

interface TransitionState {
  type: TransitionType
  easing: EasingConfig
  spring: SpringConfig
}
```

--------------------------------

### Identify Inefficient Framer Motion Animation

Source: https://motion.dev/docs/animation-performance-audit

This React component uses Framer Motion to animate 'scale', 'rotate', and 'borderRadius' properties. The audit identifies this as potentially inefficient because 'scale' and 'rotate' are animated separately, triggering multiple render pipeline stages. It serves as an example of an animation that the audit would flag for improvement.

```jsx
<motion.div
  animate={{
    scale: [1, 2, 2, 1, 1],
    rotate: [0, 0, 180, 180, 0],
    borderRadius: ["0%", "0%", "50%", "50%", "0%"],
  }}
  transition={{ repeat: Infinity }}
/>
```

--------------------------------

### Applying Easing Functions to `useTransform` (React)

Source: https://motion.dev/docs/react-use-transform

Shows how to apply custom easing functions to `useTransform` for smoother transitions between mapped values. It demonstrates using both pre-defined easing functions (`circOut`) and custom cubic Bezier functions.

```javascript
import { cubicBezier, circOut } from "motion"
import { useTransform } from "motion/react"

// In your component
const y = useTransform(x, [0, 1], [0, 2], { ease: circOut })

const z = useTransform(
  x,
  [0, 1],
  [0, 2],
  { ease: cubicBezier(0.17, 0.67, 0.83, 0.67) }
)
```

--------------------------------

### resize - Cleanup and Lifecycle

Source: https://motion.dev/docs/resize

The resize function returns a cleanup function that removes attached listeners. When all listeners are removed from an element or globally, the ResizeObserver is automatically cleaned up.

```APIDOC
## resize - Cleanup

### Description
Manage listener lifecycle and cleanup for resize observers on viewports and elements.

### Method
Function

### Signature
```javascript
const stop = resize(selector?: string | Element, callback: function): () => void
```

### Return Value
#### Cleanup Function
- **stop** (function) - Required - When called, removes the attached listener and cleans up the ResizeObserver if no other listeners remain.

### Request Example
```javascript
import { resize } from "motion"

// Viewport listener
const stopViewport = resize(() => console.log("viewport changed"))

// Element listener
const stopElement = resize(".drawer", (element, { width, height }) => {
  console.log("element changed")
})

// Remove listeners
stopViewport()
stopElement()
```

### Lifecycle Behavior
- When a listener is removed from an element, the element is removed from the ResizeObserver.
- When all listeners are removed from an element, that element is no longer observed.
- When all listeners are removed globally, the shared ResizeObserver is stopped.
- This automatic cleanup ensures optimal performance and memory usage.

### Notes
- All resize handlers share a single ResizeObserver instance for performance.
- Cleanup is automatic and does not require manual ResizeObserver management.
- Calling stop() multiple times is safe and has no additional effect after the first call.
```

--------------------------------

### Handling Element Exit from Viewport (JavaScript)

Source: https://motion.dev/docs/inview

Demonstrates how to return a function from the initial `inView` callback. This returned function will be executed when the element subsequently leaves the viewport, allowing for cleanup, stopping animations, or other exit-triggered actions.

```javascript
inView(element,
  (element, enterInfo) => {
    const animation = animate(element, { opacity: 1 })
    
    // This will fire when the element leaves the viewport
    return (leaveInfo) => animation.stop()
  }
)
```

--------------------------------

### Hardware Accelerated Scroll Animation with Motion

Source: https://motion.dev/docs/gsap-vs-motion

Demonstrates how to create a hardware accelerated scroll animation using Motion's animate and scroll functions. This approach ensures smooth animations that run on the GPU, remaining responsive even during heavy JavaScript execution. The animation applies opacity changes from 0 to 1 while scrolling.

```JavaScript
const animation = animate(element, { opacity: [0, 1] })

scroll(animation)
```

--------------------------------

### Monitor specific element size changes with resize

Source: https://motion.dev/docs/resize

Track size changes on specific elements by passing a CSS selector or element reference to resize. The callback receives the element and an object with width and height getters representing the element's border box.

```JavaScript
resize("li", (element) => console.log(element, "change detected"))

// With width and height getters
resize(".drawer", (element, { width, height }) => {
  console.log(element, " is now ", width, height)
})
```

--------------------------------

### Configuring `animate` with Options

Source: https://motion.dev/docs/animate

Configure the `animate` function with global transition options that apply to all animating values by default.

```APIDOC
## FUNCTION `animate` - Basic Options

### Description
The `animate` function accepts an options object to configure the animation's behavior, such as its duration. By default, these options apply to all properties being animated.

### Function Signature
`animate(element, keyframes, options)`

### Parameters
#### Arguments
- **element** (HTMLElement|string) - Required - The target element(s) to animate.
- **keyframes** (object) - Required - An object defining the properties and their target values.
- **options** (object) - Optional - An object containing animation configuration.

#### Options Object Properties
- **duration** (number) - Optional - The total duration of the animation in seconds.

### Example Usage
```javascript
animate(
  element,
  { x: 100, rotate: 0 },
  { duration: 1 }
)
```

### Effect/Output
The `element` will animate its `x` position to `100` and `rotate` to `0` over a period of `1` second.
```
// Element moves and rotates smoothly over 1 second.
```
```

--------------------------------

### AnimatePresence Troubleshooting

Source: https://motion.dev/docs/react-animate-presence

Common issues and solutions for AnimatePresence, including problems with exit animations and layout animations.

```APIDOC
## Troubleshooting

### Description
Common issues and solutions when working with `AnimatePresence`.

### Method
Guidance

### Endpoint
AnimatePresence

### Parameters
N/A

### Request Example
N/A

### Response
N/A

### Exit animations aren't working
Ensure all **immediate** children get a unique `key` prop that **remains the same for that component every render**.
For instance, providing `index` as a `key` is **bad** because if the items reorder then the `index` will not be matched to the `item`:

```jsx
<AnimatePresence>
  {items.map((item, index) => (
    <Component key={index} />
  ))}
</AnimatePresence>
```

It's preferred to pass something that's unique to that item, for instance an ID:

```jsx
<AnimatePresence>
  {items.map((item) => (
    <Component key={item.id} />
  ))}
</AnimatePresence>
```

Also make sure `AnimatePresence` is **outside** of the code that unmounts the element. If `AnimatePresence` itself unmounts, then it can't control exit animations!
For example, this will **not work**:

```jsx
isVisible && (
  <AnimatePresence>
    <Component />
  </AnimatePresence>
)
```

Instead, the conditional should be at the root of `AnimatePresence`:

```jsx
<AnimatePresence>
  {isVisible && <Component />}
</AnimatePresence>
```

### Layout animations not working with `mode="sync"`
When mixing exit and layout animations, it might be necessary to wrap the group in `LayoutGroup` to ensure that components outside of `AnimatePresence` know when to perform a layout animation.

```jsx
<LayoutGroup>
  <motion.ul layout>
    <AnimatePresence>
      {items.map(item => (
        <motion.li layout key={item.id} />
      ))}
    </AnimatePresence>
  </motion.ul>
</LayoutGroup>
```
```

--------------------------------

### useTransform with Sine Wave Animation

Source: https://motion.dev/docs/vue-use-transform

Uses transform function with useTime to create time-based animations. Demonstrates reading time values and applying mathematical transformations for continuous animations.

```JavaScript
const distance = 100
const time = useTime()

const y = useTransform(() => Math.sin(time.get() / 1000) * distance)
```

--------------------------------

### useInView with Initial Option

Source: https://motion.dev/docs/vue-use-in-view

Set an initial value to return before the element has been measured. Useful for preventing layout shifts or setting default animation states.

```vue
const isInView = useInView(domRef, { initial: true })
```

--------------------------------

### Customizing `springValue` Animation Physics with Options in JavaScript

Source: https://motion.dev/docs/spring-value

This snippet illustrates how to pass a configuration object as a second argument to `springValue` to customize its animation behavior. It specifically shows how to adjust the `stiffness` property, allowing fine-grained control over the spring's physics.

```javascript
springValue(0, { stiffness: 1000 })
```

--------------------------------

### useInView with Once Option in React

Source: https://motion.dev/docs/react-use-in-view

Demonstrates the once option which stops observing an element after it enters the viewport for the first time. Once triggered, the hook will always return true, useful for one-time animations or lazy loading scenarios.

```javascript
import { useInView } from "motion/react"
import { useRef } from "react"

function Component() {
  const ref = useRef(null)
  const isInView = useInView(ref, { once: true })
  
  return <div ref={ref} />
}
```

--------------------------------

### Import useTime hook from Motion library

Source: https://motion.dev/docs/vue-use-time

This snippet shows the standard way to import the `useTime` hook from the `motion-v` library. This import is necessary before `useTime` can be utilized in your JavaScript or TypeScript files.

```javascript
import { useTime } from "motion-v"
```

--------------------------------

### AnimatePresence with Dynamic Key Changes

Source: https://motion.dev/docs/react-animate-presence

Shows how AnimatePresence responds to key prop changes, triggering exit animations when the key updates. Useful for implementing slideshows and carousel components.

```jsx
<AnimatePresence>
  <Slide key={activeItem.id} />
</AnimatePresence>
```

--------------------------------

### Create Spring Motion Values with useSpring Hook

Source: https://motion.dev/docs/react-motion-value

Demonstrates how to create motion values that are attached to other motion values via a spring animation using the useSpring hook. This creates smooth, physics-based animations that follow the source values.

```javascript
const dragX = useMotionValue(0)
const dragY = useMotionValue(0)
const x = useSpring(dragX)
const y = useSpring(dragY)
```

--------------------------------

### Basic ScrambleText Component Usage in React

Source: https://motion.dev/docs/react-scramble-text

Demonstrates the fundamental usage of the `ScrambleText` component by passing text as its child. It highlights the component's core function of animating text without complex configurations.

```jsx
<ScrambleText>{text}</ScrambleText>
```

```jsx
<ScrambleText>Hello world!</ScrambleText>
```

--------------------------------

### Vue Component with Filter Motion Template

Source: https://motion.dev/docs/vue-use-motion-template

Demonstrates using useMotionTemplate in a Vue component to create a filter string with multiple motion values. The filter is applied to a motion.div element and updates reactively.

```vue
<script setup>
const blur = useMotionValue(10)
const saturate = useMotionValue(50)
const filter = useMotionTemplate`blur(${blur}px) saturate(${saturate}%)`
</script>

<template>
<motion.div :style="{ filter }" />
</template>
```

--------------------------------

### useTransform with Color Mapping

Source: https://motion.dev/docs/vue-use-transform

Maps a motion value to color values across a range. Demonstrates value mapping with color output types that Motion can animate.

```JavaScript
const x = useMotionValue(0)

const backgroundColor = useTransform(
  x,
  [0, 100],
  ["#f00", "#00f"]
)
```

--------------------------------

### Basic Element Visibility Detection with inView (JavaScript)

Source: https://motion.dev/docs/inview

Demonstrates a fundamental use case of `inView` to trigger an animation on a list item when it scrolls into the viewport. This is a common pattern for scroll-triggered effects.

```javascript
inView("#carousel li", (element) => {
  animate(element, { opacity: 1 })
})
```

--------------------------------

### Generate Motion Transition Code with toMotionTransition

Source: https://motion.dev/docs/studio-sdk-codegen

Generates a Motion transition object as a string representation that can be copy/pasted directly into Motion code. Supports spring transitions with visualDuration and bounce properties, as well as easing-based transitions.

```javascript
import { toMotionTransition } from "motion-studio"

const code = toMotionTransition(state)
/* Output:
{
  type: "spring",
  visualDuration: 0.3,
  bounce: 0.2
}
*/
```

--------------------------------

### Slideshow with dynamic key changes

Source: https://motion.dev/docs/vue-animate-presence

Create slideshow effects by changing the key prop of a single AnimatePresence child. Each key change triggers exit animation on the old component and entry animation on the new one.

```vue
<template>
  <AnimatePresence>
    <motion.img
      :key="image.src"
      :src="image.src"
      :initial="{ x: 300, opacity: 0 }"
      :animate="{ x: 0, opacity: 1 }"
      :exit="{ x: -300, opacity: 0 }"
    />
  </AnimatePresence>
</template>
```

--------------------------------

### Customize Layout Animation Transition

Source: https://motion.dev/docs/vue-layout-animations

Configures layout animation timing using the `transition` prop with duration settings. Allows fine-tuning of animation speed and easing for layout changes.

```vue
<motion.div layout :transition="{ duration: 0.3 }" />
```

--------------------------------

### Implement Staggered Text Reveal with scrambleText and stagger

Source: https://motion.dev/docs/scramble-text

Demonstrates using Motion's `stagger()` function with `scrambleText` to create a letter-by-letter reveal effect. The `startDelay` option controls when the scrambling begins for each character, adding a dynamic entry animation.

```javascript
import { scrambleText } from "motion-plus-dom"
import { stagger } from "motion"

// Start scrambling at the same time, reveal with stagger
scrambleText(element, {
  duration: stagger(0.05, { startDelay: 1 })
})
```

--------------------------------

### Initialize useAnimate and animate child elements in Vue

Source: https://motion.dev/docs/vue-use-animate

This snippet demonstrates how to import and initialize `useAnimate` within a Vue component. It uses `onMounted` to animate `li` elements that are children of the `scope` ref, ensuring animations are automatically cleaned up when the component is unmounted. The `scope` ref is applied to the `<ul>` element to define the animation context.

```vue
<script setup>
import { useAnimate } from 'motion-v'

const [scope, animate] = useAnimate()

onMounted(() => {
  // This "li" selector will only select children
  // of the element that receives `scope`
  animate('li', { opacity: 1 })
})
</script>

<template>
  <ul ref="scope">
    <slot />
  </ul>
</template>
```

--------------------------------

### AnimatePresence root Prop

Source: https://motion.dev/docs/react-animate-presence

Specifies the root element for injecting `popLayout` styles. Defaults to `document.head` but can be set to another `ShadowRoot`, for use within shadow DOM.

```APIDOC
## root

### Description
Root element for injecting `popLayout` styles. Defaults to `document.head` but can be set to another `ShadowRoot`, for use within shadow DOM.

### Method
Component Prop

### Endpoint
AnimatePresence

### Parameters
#### Request Body
- **root** (HTMLElement | ShadowRoot) - Optional - Specifies the DOM element where `popLayout` styles are injected.

### Request Example
```jsx
<AnimatePresence root={myShadowRoot}>
  {/* Children components */}
</AnimatePresence>
```

### Response
#### Success Response (N/A)
- This prop controls component behavior, not a direct API response.

#### Response Example
N/A
```

--------------------------------

### Create and Use a Steps Easing Function with Default Behavior

Source: https://motion.dev/docs/easing-functions

This snippet illustrates how to create a `steps` easing function, which produces discrete, evenly-spaced steps for animations. It demonstrates the default behavior where the step changes occur at the end of each interval, resulting in a 'jump' effect.

```javascript
import { steps } from "motion"

const easing = steps(4)

easing(0.2) // 0
easing(0.25) // 0.25
```

--------------------------------

### Apply Velocity to Scale with useTransform (React)

Source: https://motion.dev/docs/react-use-velocity

Demonstrates how to use `useVelocity` with `useMotionValue` and `useTransform` to dynamically adjust an element's scale based on its drag velocity in a React component. This allows for interactive animations where an element's visual properties react to its movement speed.

```javascript
const x = useMotionValue(0)
const xVelocity = useVelocity(x)
const scale = useTransform(
  xVelocity,
  [-3000, 0, 3000],
  [2, 1, 2],
  { clamp: false }
)

return <motion.div drag="x" style={{ x, scale }} />
```

--------------------------------

### Enable touch support with touch-action CSS

Source: https://motion.dev/docs/react-use-drag-controls

Apply touch-action: none CSS style to the triggering element to ensure proper touch screen support when initiating drag gestures from custom elements.

```javascript
<div onPointerDown={startDrag} style={{ touchAction: "none" }} />
```

--------------------------------

### Import animate from Motion Package - JavaScript

Source: https://motion.dev/docs/animate

Shows how to import the animate() function from the Motion library. Two import paths are available: the full hybrid version from 'motion' package and the lightweight mini version from 'motion/mini'.

```javascript
// Hybrid
import { animate } from "motion"

// Mini
import { animate } from "motion/mini"
```

--------------------------------

### Shared Layout Animation with Different Transitions

Source: https://motion.dev/docs/vue-layout-animations

Demonstrates how shared layout animations use the transition defined on the target element. Shows a button and dialog with different transitions for opening and closing animations.

```vue
<motion.button
  layoutId="modal"
  @click="() => isOn=true"
  :transition="{ type: 'spring' }"
>
  Open
</motion.button>
<AnimatePresence>
  <motion.dialog
    v-if="isOn"
    layoutId="modal"
    :transition="{ duration: 0.3 }"
  />
</AnimatePresence>
```

--------------------------------

### Asynchronously loading `domAnimation` features with `LazyMotion` in Vue

Source: https://motion.dev/docs/vue-lazymotion

Demonstrates how to dynamically import animation features using `import()` and then pass the resulting promise to the `features` prop of `LazyMotion`. This technique allows features to be fetched only after the initial render, optimizing bundle size for applications using bundlers like Webpack or Rollup.

```javascript
// index.js
const loadFeatures = import("./features.js")
  .then(res => res.default)
```

```html
<template>
    <LazyMotion :features="loadFeatures">
      <m.div :animate="{ scale: 1.5 }" />
    </LazyMotion>
</template>
```

--------------------------------

### EVENT /onAnimationComplete

Source: https://motion.dev/docs/vue-motion-component

No description

--------------------------------

### Applying Reduced Motion Logic in Vue Template with Motion Component

Source: https://motion.dev/docs/vue-use-reduced-motion

Illustrates the application of reduced motion logic within a Vue template using the `Motion` component. It demonstrates binding animation properties (`x`) to a computed value (`closedX`) that is derived from the `useReducedMotion` hook, ensuring animations respect user preferences.

```vue
<template>
<Motion
:animate={
opacity: isOpen ? 1 : 0,
x: isOpen ? 0 : closedX
}
/>
</template>
```

--------------------------------

### Include Custom Bundled Motion.js Script on Squarespace

Source: https://motion.dev/docs/squarespace

This HTML snippet demonstrates how to include a custom, pre-bundled JavaScript file containing Motion.js animations on a Squarespace site. After bundling Motion.js with a tool like Rollup and uploading it to a CDN, this script tag asynchronously loads the optimized file. This method further boosts SEO by reducing page load times compared to direct CDN imports.

```html
<script async src="https://yourdomain.com/my-script.js"></script>
```

--------------------------------

### Lazy load features with dynamic imports

Source: https://motion.dev/docs/react-reduce-bundle-size

Defer loading of feature packages until after initial render using dynamic imports. Create a separate features file and pass a function to LazyMotion's `features` prop that dynamically imports the file. This approach minimizes initial bundle size by loading animations and gestures only when needed.

```javascript
// features.js
import { domMax } from "motion/react"
export default domMax
```

```javascript
import { LazyMotion } from "motion/react"
import * as m from "motion/react-m"

// Make sure to return the specific export containing the feature bundle.
const loadFeatures = () =>
  import("./features.js").then(res => res.default)

// This animation will run when loadFeatures resolves.
function App() {
  return (
    <LazyMotion features={loadFeatures}>
      <m.div
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
      />
    </LazyMotion>
  )
}
```

--------------------------------

### Implement Basic Text Scrambling with motion-plus

Source: https://motion.dev/docs/scramble-text

Demonstrates how to import and use the `scrambleText` function from the `motion-plus` library to apply a text scrambling animation to a DOM element identified by a CSS selector, with a specified duration.

```javascript
import { scrambleText } from "motion-plus"

scrambleText("#title", { duration: 1 })
```

--------------------------------

### Comparing `useTransform` with `clamp: true` vs `clamp: false` (React)

Source: https://motion.dev/docs/react-use-transform

Illustrates the effect of the `clamp` option on `useTransform`. When `clamp` is `true` (default), the output is restricted to the defined range; when `false`, the mapping continues linearly beyond the range.

```javascript
const y = useTransform(x, [0, 1], [0, 2])
const z = useTransform(x, [0, 1], [0, 2], { clamp: false })

useEffect(() => {
  x.set(2)
  console.log(y.get()) // 2, input clamped
  console.log(z.get()) // 4
})
```

--------------------------------

### Monitor viewport and element resize events with Motion

Source: https://motion.dev/docs/resize

The resize function monitors size changes in the viewport or specific HTML/SVG elements. It accepts a callback function and optional CSS selector, providing width and height getters. All handlers use a shared ResizeObserver for performance optimization.

```JavaScript
// Viewport
resize(() => {})

// Specific elements
resize("li", () => {})
```

--------------------------------

### Configure Sequence Transitions - JavaScript

Source: https://motion.dev/docs/animate

Shows how to set transition options for animation sequences. Supports keyframes and spring transitions, with ability to override transitions for individual values.

```javascript
const sequence = [
  [
    "ul",
    { opacity: 1, x: 100 },
    { duration: 1, x: { duration: 2 }}
   ]
]

animate(sequence)
```

--------------------------------

### Declarative Animation Sequencing with Motion's `animate()`

Source: https://motion.dev/docs/gsap-vs-motion

This snippet presents Motion's modern, declarative alternative for animation sequencing. The `animate()` function accepts a simple JavaScript array of animation definitions, enabling easy creation, modification, and dynamic generation of complex timelines across various element types.

```javascript
animate([
  ["h1", { opacity: 1 }],
  ["p", { y: 0 }, { at: "-0.5" }]
])
```

--------------------------------

### Configure useSpring with transition options

Source: https://motion.dev/docs/react-use-spring

Customize the spring animation behavior by passing transition options like stiffness to the useSpring hook. These options control how the spring responds and animates to target values.

```javascript
useSpring(0, { stiffness: 300 })
```

--------------------------------

### Import Motion via CDN in Webflow

Source: https://motion.dev/docs/webflow

This script block imports the `animate` and `scroll` functions from the Motion library directly into a Webflow page using a CDN. It should be placed in the 'Before `<body>` tag' section of the page settings to enable basic animation functionality, such as animating the opacity of a header element.

```html
<script type="module">
  import { animate, scroll } from "https://cdn.jsdelivr.net/npm/motion@11.13.5/+esm"

  animate("header", { opacity: 1 })
</script>
```

--------------------------------

### Add exit animations to Radix with AnimatePresence

Source: https://motion.dev/docs/radix

Shows how to use Motion's AnimatePresence component to enable exit animations on Radix components. Requires conditional rendering of motion children and the forceMount prop on Radix Portal components to ensure proper animation behavior.

```jsx
<AnimatePresence>
  {isOpen && <motion.div exit={{ opacity: 0 }} />}
</AnimatePresence>
```

--------------------------------

### Apply Keyframe-Specific Easing in Motion (Vue)

Source: https://motion.dev/docs/vue-transitions

This snippet illustrates how to use an array of easing functions to apply different easings between keyframes in a `motion.div` animation. Each easing function in the array corresponds to the transition between consecutive keyframe values, allowing for nuanced motion paths.

```vue
<motion.div
  :animate="{
    x: [0, 100, 0],
    transition: { ease: ['easeIn', 'easeOut'] }
  }"
/>
```

--------------------------------

### useInView with Margin Option in React

Source: https://motion.dev/docs/react-use-in-view

Shows how to use the margin option to expand or contract the viewport detection area. Accepts CSS-style margin values (top/right/bottom/left) to adjust when elements are considered in view. Useful for triggering animations before elements become visible.

```javascript
import { useInView } from "motion/react"
import { useRef } from "react"

function Component() {
  const ref = useRef(null)
  const isInView = useInView(ref, {
    margin: "0px 100px -50px 0px"
  })
  
  return <div ref={ref} />
}
```

--------------------------------

### Subscribe to Motion Value Events with useMotionValueEvent

Source: https://motion.dev/docs/react-motion-value

Demonstrates how to listen to motion value events using the useMotionValueEvent hook. Available events include 'change', 'animationStart', 'animationComplete', and 'animationCancel'. The hook should be used instead of the on() method within React components.

```jsx
useMotionValueEvent(x, "change", (latest) => console.log(latest))
```

--------------------------------

### Basic `useTransform` Usage with Multiple Motion Values (React)

Source: https://motion.dev/docs/react-use-transform

Demonstrates the fundamental use of `useTransform` to combine the values of two `useMotionValue` instances. The resulting motion value `z` will automatically update whenever `x` or `y` change, reflecting their summed value.

```javascript
const x = useMotionValue(1)
const y = useMotionValue(1)

const z = useTransform(() => x.get() + y.get()) // z.get() === 2
```

--------------------------------

### Specifying a Custom Root Viewport for inView (JavaScript)

Source: https://motion.dev/docs/inview

Illustrates the use of the `root` option to define a specific scrollable parent element as the viewport for detection, rather than the default browser window. This is useful for detecting visibility within a confined scrolling area.

```javascript
const carousel = document.querySelector("#carousel")

inView("#carousel li", callback, { root: carousel })
```

--------------------------------

### Building Imperative Animation Timelines with GSAP

Source: https://motion.dev/docs/gsap-vs-motion

This code shows GSAP's powerful, imperative timeline function. It demonstrates creating a timeline instance and chaining multiple animation tweens with precise offsets, making it an industry standard for constructing complex and mutable animation sequences.

```javascript
const tl = gsap.timeline()
tl.to("h1", { opacity: 1 })
tl.to("p", { y: 0 }, "-=0.5")
```

--------------------------------

### Iterative Sampling of `spring` Generator in JavaScript

Source: https://motion.dev/docs/spring

This comprehensive snippet demonstrates how to continuously sample a `spring` generator in a loop until the animation is complete. It collects sampled values into an array, advancing time by a `sampleDuration` in each iteration. It also notes the need for termination conditions when `damping` is zero.

```javascript
const generator = spring({ keyframes: [25, 75], stiffness: 400 })
const output = []

let isDone = false
let time = 0
const sampleDuration = 20 // ms

while (!isDone) {
  const { value, done } = generator.next(time)

  output.push(value)

  time += sampleDuration

  if (done) isDone = true
}
```

--------------------------------

### then() Method

Source: https://motion.dev/docs/animate

A Promise-like API that resolves when the animation finishes. Supports both async/await and traditional Promise syntax. A new Promise is created each time the animation finishes.

```APIDOC
## then() Method

### Description
A `Promise`-like API that resolves when the animation finishes. When an animation finishes, a new `Promise` is created. If the animation is replayed via the `play()` method, old callbacks won't fire again.

### Method
- **then(callback)** - Registers a callback to execute when animation completes

### Usage Examples

#### Async/Await
```javascript
const animation = animate(element, { opacity: 0 })

await animation
console.log("Animation complete")
```

#### Promise
```javascript
const animation = animate(element, { opacity: 0 })

animation.then(() => {
  console.log("Animation complete")
})
```
```

--------------------------------

### AnimatePresence Basic Usage with Exit Animation

Source: https://motion.dev/docs/react-animate-presence

Demonstrates the fundamental usage of AnimatePresence wrapper with a motion component that has an exit animation prop. The component will animate out with opacity transition before being removed from the DOM.

```jsx
<AnimatePresence>
  {show && <motion.div key="modal" exit={{ opacity: 0 }} />}
</AnimatePresence>
```

--------------------------------

### AnimatePresence with List Items

Source: https://motion.dev/docs/react-animate-presence

Demonstrates AnimatePresence with a list of motion components where items are added or removed. Each item must have a unique key prop and can define exit animations.

```jsx
<AnimatePresence>
  {items.map(item => (
    <motion.li key={item.id} exit={{ opacity: 1 }} layout />
  ))}
</AnimatePresence>
```

--------------------------------

### useInView with useEffect for Side Effects in React

Source: https://motion.dev/docs/react-use-in-view

Shows how to execute functions when the isInView state changes using useEffect. This pattern allows you to trigger animations, analytics, or other side effects when an element enters or leaves the viewport.

```javascript
import { useInView } from "motion/react"
import { useRef, useEffect } from "react"

function Component() {
  const ref = useRef(null)
  const isInView = useInView(ref)
  
  useEffect(() => {
    console.log("Element is in view: ", isInView)
  }, [isInView])
  
  return <div ref={ref} />
}
```

--------------------------------

### useTransform with Value Mapping

Source: https://motion.dev/docs/vue-use-transform

Maps a single motion value from an input range to an output range. Input and output ranges must be equal length, with input values in increasing or decreasing order. Output values can be numbers, colors, units, or any animatable type.

```JavaScript
const x = useMotionValue(0)
const input = [-100, 0, 100]
const output = [0, 1, 0]

const opacity = useTransform(x, input, output)
```

--------------------------------

### Basic `transform` usage for number to color mapping (JavaScript)

Source: https://motion.dev/docs/transform

This snippet demonstrates the fundamental use of the `transform` function to map a numerical input range to a color output range. It shows how an input value within the defined range is converted into an `rgba` color representation.

```javascript
const numberToColor = transform(
[0, 100], // Input
["#000", "#fff"] // Output
)

numberToColor(50) // rgba(128, 128, 128, 1)
```

--------------------------------

### Implement hover and tap gestures on 3D motion components

Source: https://motion.dev/docs/react-three-fiber

This snippet shows how to add interactive gestures like `whileHover` and `whileTap` to a `motion.mesh` component in React Three Fiber. It also includes `onHoverStart` and `onTap` event handlers for custom side effects, enabling responsive and interactive 3D elements.

```jsx
<motion.mesh
  whileHover={{ scale: 1.1 }}
  whileTap={{ scale: 0.9 }}
  onHoverStart={() => console.log('hover start')}
  onTap={() => console.log('tapped!')}
/>
```

--------------------------------

### Basic useTransform with Transform Function

Source: https://motion.dev/docs/vue-use-transform

Creates a new motion value by applying a transform function that reads from existing motion values. The function automatically subscribes to changes and recalculates on each animation frame when dependencies update.

```JavaScript
import { useTransform, useMotionValue } from 'motion-v'

const x = useMotionValue(1)
const y = useMotionValue(1)

const z = useTransform(() => x.get() + y.get()) // z.get() === 2
```

--------------------------------

### Motion component initial prop with variants

Source: https://motion.dev/docs/react-motion-component

Use variant names as strings or arrays with the initial prop to reference predefined animation states. This enables reusable animation configurations across multiple components.

```javascript
<motion.li initial="visible" />

<motion.div initial={["visible", "active"]} />
```

--------------------------------

### Define a Basic Transition Object in JavaScript

Source: https://motion.dev/docs/vue-transitions

This snippet illustrates how to define a reusable transition object in JavaScript. It specifies common animation properties such as duration, delay, and a custom cubic bezier easing curve, which can then be applied to Motion animations.

```javascript
const transition = {
  duration: 0.8,
  delay: 0.5,
  ease: [0, 0.71, 0.2, 1.01]
}
```

--------------------------------

### Declarative Animation in React/Vue with Motion

Source: https://motion.dev/docs/gsap-vs-motion

This snippet demonstrates Motion's first-class declarative API for React and Vue. Animations are defined directly as props on components, promoting clean, readable, and maintainable code by integrating animation logic seamlessly into the component structure.

```jsx
<motion.div animate={{ x: 100 }} />
```

--------------------------------

### AnimatePresence mode prop for animation sequencing

Source: https://motion.dev/docs/vue-animate-presence

Control how AnimatePresence handles entering and exiting children using the mode prop. Options include 'sync' (default), 'wait' (sequential), and 'popLayout' (layout-aware exit).

```vue
<!-- sync mode: children animate in/out immediately -->
<AnimatePresence mode="sync">
  <Component :key="id" />
</AnimatePresence>

<!-- wait mode: entering child waits for exiting child to finish -->
<AnimatePresence mode="wait">
  <Component :key="id" />
</AnimatePresence>

<!-- popLayout mode: exiting children are popped out of layout -->
<AnimatePresence mode="popLayout">
  <Component :key="id" />
</AnimatePresence>
```

--------------------------------

### Exit Animations with Variant Labels

Source: https://motion.dev/docs/react-animate-presence

Demonstrates using variant labels for exit animations instead of inline objects. Variants allow reusable animation definitions with transition timing like 'beforeChildren' and 'afterChildren'.

```jsx
const modalVariants = {
  visible: { opacity: 1, transition: { when: "beforeChildren" } },
  hidden: { opacity: 0, transition: { when: "afterChildren" } }
}

function Modal({ children }) {
  return (
    <motion.div initial="hidden" animate="visible" exit="hidden">
      {children}
    </motion.div>
  )
}
```

--------------------------------

### Importing mapValue from Motion Library (JavaScript)

Source: https://motion.dev/docs/map-value

This snippet shows the standard way to import the `mapValue` function from the `motion` library. It is a prerequisite for using `mapValue` in any JavaScript project, making the function available for mapping motion values.

```javascript
import { mapValue } from "motion"
```

--------------------------------

### usePresence Hook for Manual Exit Control

Source: https://motion.dev/docs/react-animate-presence

Demonstrates the usePresence hook which returns isPresent state and a safeToRemove callback. Allows manual control over when a component is removed from the DOM, useful for custom animations or timeouts.

```jsx
import { usePresence } from "motion/react"

function Component() {
  const [isPresent, safeToRemove] = usePresence()

  useEffect(() => {
    // Remove from DOM 1000ms after being removed from React
    !isPresent && setTimeout(safeToRemove, 1000)
  }, [isPresent])

  return <div />
}
```

--------------------------------

### Applying Spring Animation with `animate()` in JavaScript

Source: https://motion.dev/docs/spring

This snippet demonstrates how to integrate the `spring` function as an easing type within Motion's `animate()` function. It shows how to apply a spring-based transform animation to an HTML element, configuring its bounce and duration properties.

```javascript
import { animate } from "motion/mini"
import { spring } from "motion"
  
animate(
element,
{ transform: "translateX(100px)" },
{ type: spring, bounce: 0.3, duration: 0.8 }
)
```

--------------------------------

### useInView with Custom Root Scrollable Container in React

Source: https://motion.dev/docs/react-use-in-view

Demonstrates tracking element visibility within a custom scrollable parent container instead of the window viewport. Useful for carousels, scrollable lists, or other custom scroll containers where you need to detect visibility relative to a specific parent element.

```javascript
import { useInView } from "motion/react"
import { useRef } from "react"

function Carousel() {
  const container = useRef(null)
  const ref = useRef(null)
  const isInView = useInView(ref, { root: container })
  
  return (
    <div ref={container} style={{ overflow: "scroll" }}>
      <div ref={ref} />
    </div>
  )
}
```

--------------------------------

### Initializing and Animating `springValue` with Primitives in JavaScript

Source: https://motion.dev/docs/spring-value

This snippet demonstrates how to initialize a `springValue` with a number or a string value. It shows how to update these values using the `.set()` method, triggering a physics-based spring animation. The animated values are then applied to a DOM element's style using `styleEffect`.

```javascript
const x = springValue(0)
const y = springValue("100%")

// These will go to their new target with a spring animation
x.set(100)
y.set("0%")

styleEffect("div", { x, y })
```

--------------------------------

### Exit animations with dynamic key changes

Source: https://motion.dev/docs/vue-animate-presence

Changing the key prop causes Vue to create an entirely new component, triggering exit animations on the old component. Useful for creating slideshows and carousel effects.

```vue
<AnimatePresence>
  <Slide :key="activeItem.id" />
</AnimatePresence>
```

--------------------------------

### Glide Configuration with Power Parameter

Source: https://motion.dev/docs/glide

Demonstrates the power option which controls how much initial velocity is factored into the animation distance. Higher values create lighter, further-throwing animations while lower values feel heavier.

```javascript
glide({ power: 1 })
```

--------------------------------

### Apply an array of easing functions for keyframe animations in Motion.dev

Source: https://motion.dev/docs/animate

Shows how to use an array of easing functions with the `ease` option when animating multiple keyframes. Each easing function in the array applies to the transition between consecutive keyframes.

```javascript
animate(
  element,
  { x: [0, 100, 0] },
  { ease: ["easeIn", "easeOut"] }
)
```

--------------------------------

### Duration Configuration in Seconds

Source: https://motion.dev/docs/improvements-to-the-web-animations-api-dx

Motion uses seconds for duration configuration instead of WAAPI's milliseconds, providing a more intuitive developer experience based on user testing from Framer Motion development.

```JavaScript
import { animate } from "motion/dom"

// WAAPI uses milliseconds
const waapi = element.animate({ x: 50 }, { duration: 2000 })
waapi.currentTime = 1000

// Motion uses seconds
const motion = animate(element, { x: 50 }, { duration: 2 })
motion.currentTime = 1
```

--------------------------------

### Import AnimatePresence from Motion React

Source: https://motion.dev/docs/react-animate-presence

Shows the required import statement to use AnimatePresence component in a React application with Motion library.

```jsx
import { AnimatePresence } from "motion/react"
```

--------------------------------

### useTransform with Doubled Value

Source: https://motion.dev/docs/vue-use-transform

Simple transform function that doubles a motion value. Demonstrates basic transform function usage for arithmetic operations on motion values.

```JavaScript
const x = useMotionValue(1)

const doubledX = useTransform(() => x.get() * 2)
```

--------------------------------

### Define Default Sequence Transitions - JavaScript

Source: https://motion.dev/docs/animate

Shows how to set default transition settings for all items in an animation sequence using the defaultTransition option.

```javascript
animate(sequence, {
  defaultTransition: { duration: 0.2 }
})
```

--------------------------------

### React: Importing the useTime hook from Motion

Source: https://motion.dev/docs/react-use-time

This snippet shows the necessary import statement to bring the `useTime` hook into your React component from the `motion/react` library, enabling its use for time-based animations.

```javascript
import { useTime } from "motion/react"
```

--------------------------------

### Cubic Bezier Easing with Motion Array Syntax

Source: https://motion.dev/docs/improvements-to-the-web-animations-api-dx

Uses Motion's shorthand array syntax for defining cubic bezier easing. This provides a more concise alternative to CSS string definitions while maintaining the same easing behavior.

```javascript
animate(
  element,
  { transform: "translateX(50px)" },
  { ease: [0.29, -0.13, 0.18, 1.18] }
)
```

--------------------------------

### Define and apply animation variants in Framer Motion 3D

Source: https://motion.dev/docs/react-three-fiber

This snippet illustrates how to define animation `variants` for different states (e.g., `hidden`, `visible`) and apply them to a `motion.meshStandardMaterial` component. Using `initial` and `animate` props with variants simplifies managing complex animation sequences and state transitions.

```jsx
const variants = {
  hidden: { opacity: 0 },
  visible: { opacity: 1 }
}

return (
  <motion.meshStandardMaterial
    initial="hidden"
    animate="visible"
    variants={variants}
  />
)
```

--------------------------------

### viewport - Configure Viewport Detection Options

Source: https://motion.dev/docs/react-motion-component

Defines how element visibility is tracked within the viewport. Supports options like once (fire only once), root (custom scroll container), margin (detection area adjustment), and amount (visibility threshold).

```jsx
<motion.section
  whileInView={{ opacity: 1 }}
  viewport={{ once: true }}
/>
```

--------------------------------

### Spring animation with Vue reactive reference

Source: https://motion.dev/docs/css

Create reactive spring animations in Vue using ref() to store the spring value, then bind it to element styles using v-bind directive for dynamic transitions.

```javascript
const springTransition = ref(spring(0.3, 1))
```

```javascript
<div :style="{ transition: 'filter ' + springTransition }"></div>
```

--------------------------------

### Separate Layout and Default Transitions

Source: https://motion.dev/docs/vue-layout-animations

Specifies different transitions for layout animations versus other property animations. The `layout` key in the transition object applies only to layout changes, while `default` applies to other animations like opacity.

```vue
<motion.div
  layout
  :animate="{ opacity: 0.5 }"
  :transition="{
    default: { ease: 'linear' },
    layout: { duration: 0.3 }
  }"
/>
```

--------------------------------

### BezierCurveEditor Props Reference

Source: https://motion.dev/docs/studio-sdk-bezier-curve-editor

Detailed reference for all available props for customizing the BezierCurveEditor component.

```APIDOC
## PROPS BezierCurveEditor

### Description
This section details all the props available for the `BezierCurveEditor` component, allowing for customization of its behavior and appearance.

### Method
React Component Props

### Endpoint
N/A (React Component)

### Parameters
#### Props
- **curve** (array) - Required - An array of four numbers representing the bezier curve points `[x1, y1, x2, y2]`. This prop controls the current state of the curve.
    *   **Example:** `[0.3, 0, 0.6, 1]`
- **onChange** (function) - Required - A callback function that is invoked when the curve is updated by user interaction. It receives the new curve array as its argument.
    *   **Example:** `(newCurve) => setCurve(newCurve)`
- **color** (string) - Optional - Default: `#fff` - Defines the color used for the curve visualization, control points, and their focus rings.
- **pathWidth** (number) - Optional - Default: `3` - Specifies the stroke width of the bezier curve path.
- **axisColor** (string) - Optional - Default: `#fff` - Sets the color of the x/y axis lines displayed in the editor.
- **axisWidth** (number) - Optional - Default: `3` - Sets the stroke width of the x/y axis lines.
- **controlRadius** (number) - Optional - Default: `7` - Determines the visual radius of the draggable control handles.
- **hitRadius** (number) - Optional - Default: `40` - Defines the radius of the invisible, oversized hit areas around control points, enhancing touch accessibility.
- **tetherWidth** (number) - Optional - Default: `2` - Sets the stroke width of the lines connecting control points to the curve.
- **tetherDashArray** (string) - Optional - Default: `"4, 2"` - Specifies the SVG `stroke-dasharray` property for the tether lines, e.g., `"4, 2"` for a dashed line.
- **debug** (boolean) - Optional - If set to `true`, the oversized hit points for touch accessibility will be visually rendered, aiding in debugging.

### Request Example
```javascript
<BezierCurveEditor
  curve={[0.2, 0.8, 0.8, 0.2]}
  onChange={handleCurveChange}
  color="blue"
  pathWidth={4}
  axisColor="gray"
  controlRadius={10}
  hitRadius={50}
  tetherWidth={3}
  tetherDashArray="8, 4"
  debug={true}
/>
```

### Response
#### N/A (React Component)
Props configure the component's behavior and appearance; they do not directly result in a "response" in the API sense.

#### Response Example
N/A
```

--------------------------------

### Animate Element Interactions with Motion.js `press` on Squarespace

Source: https://motion.dev/docs/squarespace

This JavaScript snippet demonstrates how to use Motion.js's `press` function to create interactive animations on Squarespace. It scales down `<a>` elements when they are pressed and scales them back to their original size when released, providing visual feedback for user interactions. This requires importing both `animate` and `press` from the Motion.js library.

```html
<script type="module" defer>
    import { animate, press } from "https://cdn.jsdelivr.net/npm/motion@11.13.5/+esm"

    press("a", (element) => {
      animate(element, { scale: 0.7 })

      return () => animate(element, { scale: 1 })
    })
</script>
```

--------------------------------

### attrEffect with CSS Selector and Data Attributes

Source: https://motion.dev/docs/attr-effect

Demonstrates applying a motion value to a data attribute using a CSS selector. The progress motion value is bound to the data-progress attribute and will update the element on each animation frame.

```javascript
const progress = motionValue(0.5)

attrEffect("#progress", { "data-progress": progress })
```

--------------------------------

### Dynamic exit animations with custom prop

Source: https://motion.dev/docs/vue-animate-presence

Pass a value through the custom prop to enable dynamic variants that change exit animations based on external state. Useful when component props cannot be updated during removal.

```vue
<script setup>
  const variants = {
    hidden: (direction) => ({
      opacity: 0,
      x: direction === 1 ? -300 : 300
    }),
    visible: { opacity: 1, x: 0 }
  }
</script>

<template>
  <AnimatePresence :custom="direction">
    <motion.img
      :key="image.src"
      :src="image.src"
      :variants="variants"
      initial="hidden"
      animate="visible"
      exit="hidden"
    />
  </AnimatePresence>
</template>
```

--------------------------------

### useTransform with Unclamped Range Mapping

Source: https://motion.dev/docs/vue-use-transform

Uses clamp: false option to enable perpetual range mapping beyond the defined input range. Useful for continuous transformations like infinite rotation based on scroll distance.

```JavaScript
const { scrollY } = useScroll()

const rotate = useTransform(
  scrollY,
  [0, 100],
  [0, 360],
  { clamp: false }
)
```

--------------------------------

### Callbacks in Animation Sequences

Source: https://motion.dev/docs/animate

Learn how to insert callback functions into animation sequences to perform actions at specific points, either based on progress or custom keyframes.

```APIDOC
## FUNCTION `animate` - Callbacks

### Description
Callback functions can be inserted into animation sequences to react to animation progress or specific keyframe values.

### Function Signature
`animate(target, keyframes, options)` (Implicitly, the keyframes can contain callbacks)

### Parameters
#### Keyframes (Callback Usage)
- **callback** (function) - Required - A function that receives the latest animated value or progress.
- **keyframes_array** (array) - Optional - An array of values to pass to the callback function over the animation duration.

### Example Usage
```javascript
const sequence = [
  [(latest) => console.log(latest)]
]
// Outputs progress (0 to 1)

const sequenceWithCustomKeyframes = [
  [(color) => console.log(color), ["#000", "#fff"]]
]
// Outputs custom keyframe values
```

### Effect/Output
The callback function is executed during the animation, logging either the progress (0-1) or custom keyframe values to the console.
```
// Example output for progress callback
0.1
0.2
...
1

// Example output for custom keyframes
#000
#333
...
#fff
```
```

--------------------------------

### Glide Animation with Min and Max Boundaries

Source: https://motion.dev/docs/glide

Illustrates how to constrain glide animations within minimum and maximum boundaries. When the animated value exceeds these boundaries, a spring animation automatically takes over to snap the value back to the boundary.

```javascript
glide({ min: -100, max: 100 })
```

--------------------------------

### Import press function from Motion

Source: https://motion.dev/docs/press

Import the press gesture detection function from the Motion library. This is the first step to using press gestures in your project.

```javascript
import { press } from "motion"
```

--------------------------------

### Mapping Numerical Motion Values to Numbers and Colors (JavaScript)

Source: https://motion.dev/docs/map-value

This snippet demonstrates how to use `mapValue` to create new motion values that map an input numerical motion value to different ranges, including numerical opacity and color values. It shows chaining `mapValue` calls to achieve complex animations based on a single input motion value.

```javascript
const x = motionValue(100)

// Fade out outside the 0-100 range
const opacity = mapValue(x, [-100, 0, 100, 200], [0, 1, 1, 0])

// Shift color when fading out
const backgroundColor = mapValue(opacity, [0, 1], ["#f00", "#00f"])
```

--------------------------------

### Configure global animation options in Motion.dev

Source: https://motion.dev/docs/animate

Demonstrates how to apply global transition options, such as `duration`, to all animating values within a single `animate` call. These options affect every property being animated.

```javascript
animate(
  element,
  { x: 100, rotate: 0 },
  { duration: 1 }
)
```

--------------------------------

### Import lightweight m component instead of motion

Source: https://motion.dev/docs/react-reduce-bundle-size

Replace the full `motion` component with the slimmer `m` component from 'motion/react-m'. The `m` component provides the same API as `motion` but without preloaded features like animations, layout animations, or drag gestures, reducing bundle size to approximately 4.6kb.

```javascript
import * as m from "motion/react-m"
```

--------------------------------

### Motion container with animated child elements in React

Source: https://motion.dev/docs/figma

Demonstrates a Motion component structure using variants for container and child animations. The container uses initial and animate props to control animation states, while child elements are mapped and individually animated with variants. This pattern is commonly generated by Figma Make for staggered animations.

```jsx
<motion.div
  className={className}
  variants={container}
  initial="hidden"
  animate="visible"
>
  {words.map((word, index) => (
    <motion.span
      key={index}
      variants={child}
      style={{ display: "inline-block", marginRight: "0.25em" }}
    >
      {word}
    </motion.span>
  ))}
</motion.div>
```

--------------------------------

### Importing useReducedMotion Hook from Motion-v

Source: https://motion.dev/docs/vue-use-reduced-motion

Provides the necessary import statement for the `useReducedMotion` hook from the `motion-v` library. This line should be included at the top of any JavaScript or TypeScript file where the hook is intended to be used.

```javascript
import { useReducedMotion } from "motion-v"
```

--------------------------------

### Import spring function from Motion

Source: https://motion.dev/docs/css

Import the spring function from the Motion library to generate CSS spring animations. This is the primary entry point for creating spring-based transitions in CSS.

```javascript
import { spring } from "motion"
```

--------------------------------

### Import AnimatePresence from motion-v

Source: https://motion.dev/docs/vue-animate-presence

Import the AnimatePresence component from the motion-v library to enable exit animations in Vue applications.

```javascript
import { AnimatePresence } from "motion-v"
```

--------------------------------

### Create and Use Motion Value with useMotionValue Hook

Source: https://motion.dev/docs/react-motion-value

Demonstrates how to create a motion value manually using the useMotionValue hook and apply it to a motion component via the style prop. The motion value tracks state and can be rendered efficiently without triggering React re-renders.

```jsx
import { motion, useMotionValue } from "motion/react"

export function MyComponent() {
  const x = useMotionValue(0)
  return <motion.div style={{ x }} />
}
```

--------------------------------

### React App Component with Framer Motion MotionConfig

Source: https://motion.dev/docs/react-three-fiber

Main App component that sets up Framer Motion configuration and manages fullscreen state. It wraps the Scene component with MotionConfig to apply consistent transition settings across all animations. The component toggles fullscreen mode on click.

```javascript
import "./styles.css";
import { useState, Suspense } from "react";
import { motion, MotionConfig } from "framer-motion";
import { Scene } from "./Scene";
import { transition } from "./settings";

export default function App() {
  const [isFullscreen, setFullscreen] = useState(false);
  return (
    <MotionConfig transition={transition}>
      <div
        data-is-fullscreen={isFullscreen}
        onClick={() => setFullscreen(!isFullscreen)}
      >
        {/* Scene component and content */}
      </div>
    </MotionConfig>
  );
}
```

--------------------------------

### Basic Glide Animation with Momentum Physics

Source: https://motion.dev/docs/glide

Demonstrates the fundamental usage of glide() easing to animate an element's x position using momentum physics. The glide function automatically calculates the animation target and duration based on initial velocity and physics parameters.

```javascript
import { animate, glide } from "motion"

animate(
  element,
  { x: 500 },
  { easing: glide() }
)
```

--------------------------------

### Remove resize listeners and cleanup ResizeObserver

Source: https://motion.dev/docs/resize

The resize function returns a cleanup function that removes attached listeners. When no listeners remain on an element, it is removed from the ResizeObserver, and the observer stops when all listeners are removed.

```JavaScript
const stop = resize(log)
stop()
```

--------------------------------

### Apply `whileHover` and `whilePress` Animations in Vue

Source: https://motion.dev/docs/vue-gestures

This snippet demonstrates how to use the `whileHover` and `whilePress` props on a `motion.button` component to define direct animation targets. It shows animating `scale` with a `transition` duration on hover and a simple `scale` change on press.

```html
<motion.button
  :whileHover="{
    scale: 1.2,
    transition: { duration: 1 }
  }"
  :whilePress="{ scale: 0.9 }"
/>
```

--------------------------------

### One-time Callbacks with Cleanup (`toggle` helper)

Source: https://motion.dev/docs/animate

Implement one-time actions with a cleanup mechanism for scrubbable and reversible animations using a `toggle` helper function.

```APIDOC
## FUNCTION `animate` - `toggle` Helper

### Description
The `toggle` helper function allows for executing a function once when an animation reaches its end (forwards) and another function when it reverses past that point (backwards), providing a cleanup mechanism essential for stateless and scrubbable animations.

### Function Signature
`toggle(onForwards, onBackwards)`

### Parameters
#### Arguments for `toggle`
- **onForwards** (function) - Required - Function to execute when animation completes forwards.
- **onBackwards** (function) - Required - Function to execute when animation reverses past the completion point.

### Example Usage
```javascript
function toggle(onForwards, onBackwards) {
  let done = false
  
  return (p) => {
    if (p >= 1 && !done) { done = true; onForwards() }
    else if (p < 1 && done) { done = false; onBackwards() }
  }
}

animate([
  [
    toggle(
      () => el.classList.add("active"),
      () => el.classList.remove("active")
    ),
    { duration: 0 }
  ]
])
```

### Effect/Output
When the animation completes (progress `p` reaches 1), `el` gets the "active" class. If the animation reverses or is cancelled before completion, the "active" class is removed.
```
// When animation completes
<div class="el active">...</div>

// When animation reverses
<div class="el">...</div>
```
```

--------------------------------

### Generating CSS Transition String with `spring()` in JavaScript

Source: https://motion.dev/docs/spring

This snippet shows how the `spring()` function can be directly used to generate a CSS transition string. This string can then be assigned to an element's `transition` style property, enabling spring-based CSS animations.

```javascript
element.style.transition = "all " + spring(0.5)
```

--------------------------------

### Basic Ticker Component Usage in Vue

Source: https://motion.dev/docs/vue-ticker

This snippet demonstrates the most basic usage of the Ticker component within a Vue template. It shows how to wrap simple content directly inside the `<Ticker>` tags to create an infinitely scrolling marquee effect.

```html
<Ticker>
😂
</Ticker>
```

--------------------------------

### Troubleshooting AnimatePresence Exit Animations (React)

Source: https://motion.dev/docs/react-animate-presence

To ensure exit animations work correctly with AnimatePresence, immediate children must have a unique and stable `key` prop (not an array index). Additionally, AnimatePresence itself must remain mounted and not be conditionally rendered, instead, its children should be conditional.

```jsx
// Bad: Using index as key, which can cause issues if items reorder
<AnimatePresence>
  {items.map((item, index) => (
    <Component key={index} />
  ))}
</AnimatePresence>
```

```jsx
// Good: Using a unique item ID as key
<AnimatePresence>
  {items.map((item) => (
    <Component key={item.id} />
  ))}
</AnimatePresence>
```

```jsx
// Bad: AnimatePresence unmounts with the conditional
isVisible && (
  <AnimatePresence>
    <Component />
  </AnimatePresence>
)
```

```jsx
// Good: AnimatePresence remains mounted, only its children are conditional
<AnimatePresence>
  {isVisible && <Component />}
</AnimatePresence>
```

--------------------------------

### Cubic Bezier Easing with WAAPI

Source: https://motion.dev/docs/improvements-to-the-web-animations-api-dx

Defines cubic bezier easing as a CSS string in WAAPI. This syntax is compatible with Motion but Motion also provides a shorthand array syntax for easier definition.

```javascript
element.animate(
  { transform: "translateX(50px)" },
  { easing: "cubic-bezier(0.29, -0.13, 0.18, 1.18)" }
)
```

--------------------------------

### Import Typewriter Component in React

Source: https://motion.dev/docs/react-typewriter

Shows how to import the `Typewriter` component from the `motion-plus/react` module. This step is necessary to make the component available for use within a React application.

```jsx
import { Typewriter } from "motion-plus/react"
```

--------------------------------

### Apply Motion Values to Data Object Properties

Source: https://motion.dev/docs/prop-effect

propEffect accepts a data object and a map of motion values to apply. When motion values update via set(), the properties are automatically synchronized on the next animation frame.

```javascript
const data = { opacity: 0, x: 100 }
const opacity = motionValue(0)

propEffect(data, { opacity })

when any of the motion values update, the element(s) will re-render on the next animation frame:
opacity.set(1)
```

--------------------------------

### Perform a Crossfade View Animation with Motion+ JavaScript

Source: https://motion.dev/docs/animate-view

This snippet demonstrates a basic crossfade animation using Motion's `animateView()` function. It shows how to define an 'enter' animation for a new view, setting its `opacity` to `1` to create a smooth fade-in effect. This function simplifies animating between different views or layouts, building upon the native View Transition API.

```javascript
// Crossfade
animateView(update).enter({ opacity: 1 })
```

--------------------------------

### Configure Animation Repetition in Framer Motion

Source: https://motion.dev/docs/vue-transitions

Sets the number of times an animation should repeat. Use `Infinity` for continuous looping. Default is 0, meaning no repetition.

```Framer Motion
<motion.div
  :animate="{ rotate: 180 }"
  :transition="{ repeat: Infinity, duration: 2 }"
/>
```

--------------------------------

### Fix layout animations with popLayout mode using relative positioning

Source: https://motion.dev/docs/react-animate-presence

Demonstrates how to properly configure a motion.ul container with layout animations and popLayout mode. The parent element uses position: "relative" to ensure child elements with position: "absolute" are positioned correctly relative to the parent, not the document. This prevents positioning issues when the parent has active transforms.

```jsx
<motion.ul layout style={{ position: "relative" }}>
  <AnimatePresence mode="popLayout">
    {items.map(item => (
      <motion.li layout key={item.id} />
    ))}
  </AnimatePresence>
</motion.ul>
```

--------------------------------

### MotionConfig Component Configuration

Source: https://motion.dev/docs/react-motion-config

The MotionConfig component wraps child motion components and applies configuration options globally. It accepts props for transition defaults, reduced motion handling, and CSP nonce attributes to control animation behavior across your application.

```APIDOC
## MotionConfig Component

### Description
The MotionConfig component sets configuration options for all child motion components, providing a context-based approach to managing animation behavior site-wide.

### Usage
```jsx
import { motion, MotionConfig } from "motion/react"

export const MyComponent = ({ isVisible }) => (
  <MotionConfig transition={{ duration: 1 }}>
    <motion.div
      initial={{ opacity: 0 }}
      animate={{ opacity: 1 }}
    />
  </MotionConfig>
)
```

### Props

#### transition
- **Type:** `Transition` - Optional
- **Description:** Defines a fallback transition to use for all child motion components. This transition will be applied to any child motion component that does not have its own transition defined.

#### reducedMotion
- **Type:** `"user" | "always" | "never"` - Optional
- **Default:** `"never"`
- **Description:** Sets a site-wide policy for handling reduced motion preferences. Accepts three options:
  - `"user"`: Respects the user's device setting for reduced motion
  - `"always"`: Enforces reduced motion (useful for debugging)
  - `"never"`: Does not respect reduced motion settings
- **Behavior:** When reduced motion is enabled, transform and layout animations are disabled. Other animations like opacity and backgroundColor persist.

#### nonce
- **Type:** `string` - Optional
- **Description:** If using a Content Security Policy with a nonce attribute, pass the same nonce value through MotionConfig. This allows any style blocks generated by Motion to adhere to the security policy.

### Request Example
```jsx
<MotionConfig 
  transition={{ duration: 1, ease: "easeInOut" }}
  reducedMotion="user"
  nonce="abc123xyz"
>
  <motion.div
    initial={{ opacity: 0 }}
    animate={{ opacity: 1 }}
  />
</MotionConfig>
```

### Response Behavior
- All child motion components inherit the configuration from MotionConfig
- Child components can override inherited settings with their own props
- Reduced motion settings affect transform and layout animations globally
- CSP nonce is applied to all generated style blocks
```

--------------------------------

### Cancel a Motion `frame` callback

Source: https://motion.dev/docs/frame

This snippet illustrates how to import both `frame` and `cancelFrame` to manage scheduled callbacks. It shows scheduling a function to run during the `read` phase and then immediately cancelling it, preventing its execution.

```javascript
import { frame, cancelFrame } from "framer-motion"

function measureElement() {
  console.log(element.getBoundingClientRect())
}

frame.read(measureElement)
cancelFrame(measureElement)
```

--------------------------------

### Update Motion Values with attrEffect

Source: https://motion.dev/docs/attr-effect

Shows how to update motion values after they have been bound to element attributes with attrEffect. Changes to the motion value trigger re-rendering on the next animation frame.

```javascript
progress.set(1)
animate(progress, 1)
```

--------------------------------

### Glide Animation with Bounce Stiffness Configuration

Source: https://motion.dev/docs/glide

Shows how to configure bounceStiffness which controls the attraction force of the spring used when animation exceeds min/max boundaries. Higher values create faster, sharper bounce-back movement.

```javascript
glide({ min: 100, bounceStiffness: 500 })
```

--------------------------------

### Create Animation Sequences - JavaScript

Source: https://motion.dev/docs/animate

Shows how to create complex animation sequences using an array of animate definitions. Each definition plays sequentially by default, with support for timing control via the 'at' option.

```javascript
const sequence = [
  ["ul", { opacity: 1 }, { duration: 0.5 }],
  ["li", 100, { ease: "easeInOut" }]
]

animate(sequence)
```

--------------------------------

### Create useSpring with number or unit string

Source: https://motion.dev/docs/react-use-spring

Initialize useSpring with either a numeric value or a unit-type string (px, %, vh, etc). The motion value will animate to new targets using spring physics when updated via the .set() method.

```javascript
const x = useSpring(0)
const y = useSpring("100vh")
```

--------------------------------

### Import useMotionValueEvent Hook for React Motion

Source: https://motion.dev/docs/react-use-motion-value-event

This snippet provides the standard import statement for integrating the `useMotionValueEvent` hook into a React application using the Motion library.

```javascript
import { useMotionValueEvent } from "motion/react"
```

--------------------------------

### Define Motion spring animation with bounce parameter

Source: https://motion.dev/docs/studio-generate-css

Motion spring configuration object using type and bounce parameters. This represents a maintainable alternative to CSS linear() curves, allowing easy tweaking of spring bounciness and duration. The bounce parameter controls oscillation after reaching target value, with visualDuration determining the apparent animation time.

```javascript
{ type: "spring", bounce: 0.2 }
```

--------------------------------

### Configure Animation Repeat Type Parameter

Source: https://motion.dev/docs/animate

Defines how animations repeat with a default value of 'loop'. Options include: 'loop' (restart from beginning), 'reverse' (alternate forward/backward), and 'mirror' (switch animation origin and target). Controls the playback behavior during repetitions.

```javascript
animate(
  element,
  { backgroundColor: "#fff" },
  { repeat: 1, repeatType: "reverse", duration: 2 }
)
```

--------------------------------

### Implement a toggle helper for one-time actions in scrubbable Motion.dev animations

Source: https://motion.dev/docs/animate

Provides a `toggle` helper function to manage one-time actions (like adding/removing a class) in stateless, scrubbable animations. It ensures actions are performed only once when progressing forwards or backwards, with cleanup.

```javascript
function toggle(onForwards, onBackwards) {
  let done = false
  
  return (p) => {
    if (p >= 1 && !done) { done = true; onForwards() }
    else if (p < 1 && done) { done = false; onBackwards() }
  }
}

animate([
  [
    toggle(
      () => el.classList.add("active"),
      () => el.classList.remove("active")
    ),
    { duration: 0 }
  ]
])
```

--------------------------------

### Exit animations using variant labels

Source: https://motion.dev/docs/vue-animate-presence

Define exit animations as variant labels instead of inline objects. Variants support transition timing options like 'beforeChildren' and 'afterChildren'.

```vue
<script setup>
  const modalVariants = {
    visible: { opacity: 1, transition: { when: "beforeChildren" } },
    hidden: { opacity: 0, transition: { when: "afterChildren" } }
  }
</script>

<template>
  <motion.div 
    :variants="modalVariants"
    initial="hidden" 
    animate="visible" 
    exit="hidden"
  >
    {{children}}
  </motion.div>
</template>
```

--------------------------------

### Spring animation with Styled Components

Source: https://motion.dev/docs/css

Integrate spring animations with Styled Components CSS-in-JS library by embedding the spring() function directly in template literals for styled component definitions.

```javascript
const Button = styled.button`
  transition: opacity ${spring(0.5)};
`
```

--------------------------------

### Vue Cursor Component with Follow Effect

Source: https://motion.dev/docs/vue-cursor

This snippet illustrates how to activate a 'follow' effect for the Motion+ Cursor component using a simple prop. This feature is ideal for creating visual trails or attaching interactive elements that follow the cursor's movement, enhancing user engagement.

```Vue
<Cursor follow />
```

--------------------------------

### Basic BezierCurveEditor Component Usage (React)

Source: https://motion.dev/docs/studio-sdk-bezier-curve-editor

This snippet demonstrates the fundamental way to render the `BezierCurveEditor` React component. It requires a `curve` prop, which defines the bezier points, and an `onChange` handler to update the curve's state when user interactions occur.

```jsx
<BezierCurveEditor curve={curve} onChange={setCurve} />
```

--------------------------------

### Generate CSS Transition String with toCSSTransition

Source: https://motion.dev/docs/studio-sdk-codegen

Generates a partial CSS transition definition from a TransitionState object. Returns a string containing duration and easing function that can be used in CSS transition properties. Supports bezier curves, and spring animations are converted to linear() easing curves.

```javascript
import { toCSSTransition } from "motion-studio"

const cssString = toCSSTransition(state)
// Output: "0.3s cubic-bezier(0.3, 0.05, 0.45, 1)"

// Use in CSS transition definition
`transition: opacity ${cssString}`
```

--------------------------------

### Sampling `spring` Generator Values in JavaScript

Source: https://motion.dev/docs/spring

This snippet demonstrates how to retrieve the current value and completion status from a `spring` generator at a specific millisecond timestamp using the `next()` method. The `value` property holds the spring's state, and `done` indicates if the animation is complete.

```javascript
const { value, done } = generator.next(10)
```

--------------------------------

### Import BezierCurveEditor Component (JavaScript)

Source: https://motion.dev/docs/studio-sdk-bezier-curve-editor

This snippet illustrates how to import the `BezierCurveEditor` component from the `motion-studio` package. This import statement is essential for making the component available for use within a React application.

```javascript
import { BezierCurveEditor } from "motion-studio"
```

--------------------------------

### Set Sequence Duration and Playback - JavaScript

Source: https://motion.dev/docs/animate

Demonstrates how to manually set sequence duration and control overall playback settings like repeat count. Sequence durations are automatically calculated but can be overridden.

```javascript
animate(sequence, { duration: 10, repeat: 2 })
```

--------------------------------

### Import hover function from Motion

Source: https://motion.dev/docs/hover

Import the hover gesture detection function from the Motion library to use in your project.

```javascript
import { hover } from "motion"
```

--------------------------------

### Import useSpring from Motion/React

Source: https://motion.dev/docs/react-use-spring

Import the useSpring hook from the Motion library to enable spring animations in React components. This is the first step to using spring-based motion values in your application.

```javascript
import { useSpring } from "motion/react"
```

--------------------------------

### BezierCurveEditor Component Overview

Source: https://motion.dev/docs/studio-sdk-bezier-curve-editor

An overview of the BezierCurveEditor React component, its purpose, and basic usage.

```APIDOC
## COMPONENT BezierCurveEditor

### Description
`BezierCurveEditor` is a React input component designed to edit bezier easing curve definitions. It is highly customizable, keyboard, and touch accessible, providing a robust solution for animation curve manipulation.

### Method
React Component

### Endpoint
N/A (React Component)

### Parameters
#### Props
- **curve** (array) - Required - An array of valid bezier curve points, e.g., `[0.3, 0, 0.6, 1]`.
- **onChange** (function) - Required - A callback function triggered when the bezier curve is updated, receiving the new curve state.
- **color** (string) - Optional - Default: `#fff` - Sets the color of the curve visualization, control points, and focus rings.
- **pathWidth** (number) - Optional - Default: `3` - Sets the path width of the curve visualization.
- **axisColor** (string) - Optional - Default: `#fff` - Sets the color of the x/y axis lines.
- **axisWidth** (number) - Optional - Default: `3` - Sets the width of the x/y axis lines.
- **controlRadius** (number) - Optional - Default: `7` - Sets the radius of the control handles.
- **hitRadius** (number) - Optional - Default: `40` - Sets the radius of the control handle hit points for touch accessibility.
- **tetherWidth** (number) - Optional - Default: `2` - Sets the width of the path tethering control handles to the curve.
- **tetherDashArray** (string) - Optional - Default: `"4, 2"` - Sets the `dasharray` of the path tethering control handles.
- **debug** (boolean) - Optional - If `true`, visualizes hit points for debugging touch accessibility.

### Request Example
```javascript
import { BezierCurveEditor } from "motion-studio";
import React, { useState } from "react";

function MyComponent() {
  const [curve, setCurve] = useState([0.3, 0, 0.6, 1]);

  return (
    <BezierCurveEditor
      curve={curve}
      onChange={setCurve}
      color="#FF0000"
      pathWidth={5}
      debug={true}
    />
  );
}
```

### Response
#### N/A (React Component)
The component renders UI and manages internal state, providing updates via the `onChange` prop.

#### Response Example
N/A
```

--------------------------------

### useInView with Once Option

Source: https://motion.dev/docs/vue-use-in-view

Enable the once option to stop observing an element after it enters the viewport for the first time. The hook will always return true after the initial detection.

```vue
const isInView = useInView(domRef, { once: true })
```

--------------------------------

### Retrieving Reduced Motion Preference with useReducedMotion Hook

Source: https://motion.dev/docs/vue-use-reduced-motion

Demonstrates how to call the `useReducedMotion` hook to obtain the user's reduced motion preference. The returned boolean value can then be used to conditionally alter UI behavior or animations, adapting to accessibility settings.

```javascript
const shouldReduceMotion = useReducedMotion()
```

```javascript
const prefersReducedMotion = useReducedMotion()
```

--------------------------------

### ScrambleText with Custom Binary Characters in React

Source: https://motion.dev/docs/react-scramble-text

Illustrates how to specify a custom set of characters for the scrambling animation by passing a string (e.g., '01' for a binary effect) to the `chars` prop of the `ScrambleText` component.

```jsx
// Binary effect
<ScrambleText chars="01" duration={1}>Hello</ScrambleText>
```

--------------------------------

### Motion component transition prop

Source: https://motion.dev/docs/react-motion-component

Define the default transition configuration for a motion component. This transition applies to all animation props (animate, whileHover, etc.) that don't have their own transition defined. Supports spring, tween, and other transition types.

```javascript
<motion.div transition={{ type: "spring" }} animate={{ scale: 1.2 }} />
```

--------------------------------

### AnimatePresence custom Prop

Source: https://motion.dev/docs/react-animate-presence

Allows passing dynamic data to children's exit animations via variants, enabling more flexible animation control.

```APIDOC
## custom

### Description
When a component is removed, there's no longer a chance to update its props (because it's no longer in the React tree). Therefore we can't update its exit animation with the same render that removed the component.
By passing a value through `AnimatePresence`'s `custom` prop, we can use dynamic variants to change the `exit` animation.

### Method
Component Prop

### Endpoint
AnimatePresence

### Parameters
#### Request Body
- **custom** (any) - Optional - A value that can be accessed by children via `usePresenceData` to influence dynamic variants for exit animations.

### Request Example
```jsx
const variants = {
  hidden: (direction) => ({
    opacity: 0,
    x: direction === 1 ? -300 : 300
  }),
  visible: { opacity: 1, x: 0 }
}

export const Slideshow = ({ image, direction }) => (
  <AnimatePresence custom={direction}>
    <motion.img
      key={image.src}
      src={image.src}
      variants={variants}
      initial="hidden"
      animate="visible"
      exit="hidden"
    />
  </AnimatePresence>
)
```

### Response
#### Success Response (N/A)
- This prop controls component behavior, not a direct API response.

#### Response Example
N/A
```

--------------------------------

### Basic AnimatePresence with exit animation

Source: https://motion.dev/docs/vue-animate-presence

Wrap motion components with AnimatePresence to gain access to the exit animation prop. Direct children must have unique key props for AnimatePresence to track their presence.

```vue
<AnimatePresence>
  <motion.div v-if="show" key="modal" :exit="{ opacity: 0 }" />
</AnimatePresence>
```

--------------------------------

### Listen for Motion Value 'change' Event in React

Source: https://motion.dev/docs/react-use-motion-value-event

This code illustrates how to use `useMotionValueEvent` to subscribe to the 'change' event of a `useMotionValue`. The callback function receives the `latest` value, which is then logged to the console, demonstrating real-time value tracking.

```javascript
const color = useMotionValue("#00f")

useMotionValueEvent(color, "change", (latest) => {
  console.log(latest)
})
```

--------------------------------

### Create Continuous Text Scrambling with Infinite Duration

Source: https://motion.dev/docs/scramble-text

Explains how to set `duration` to `Infinity` for `scrambleText` to achieve a continuous scrambling effect. It also shows how to control the animation using `finish()` or `stop()` on hover, providing interactive control over infinite animations.

```javascript
hover(element, () => {
  const controls = scrambleText(element, { duration: Infinity })

  return () => {
    controls.finish() // Reveal while preserving stagger
    // or controls.stop() for immediate reveal
  }
})
```

--------------------------------

### Defining Responsive Initial Animation Values with CSS Variables (React/Tailwind CSS)

Source: https://motion.dev/docs/react-tailwind

This snippet illustrates how to make animations responsive by combining Tailwind CSS's ability to set responsive CSS variables with Motion's capability to animate them. It defines a CSS variable `--entry-distance-y` with different values for small and medium screens, used as an initial animation state.

```html
<motion.div
  className="
    p-8 bg-rose-500 text-white rounded-xl shadow-lg max-w-md mx-auto
    
    /* Define the CSS variable inline, with responsive values */
    [--entry-distance-y:20px] 
    md:[--entry-distance-y:50px]
  "
  initial={{ opacity: 0, y: "var(--entry-distance-y)" }}
```

--------------------------------

### Layout Animation in Fixed Containers

Source: https://motion.dev/docs/vue-layout-animations

Applies the `layoutRoot` prop to fixed-position elements to correctly measure child layout animations. This accounts for the page's scroll offset when calculating layout changes.

```vue
<motion.div layoutRoot :style="{ position: 'fixed' }" />
```

--------------------------------

### Glide Animation with Bounce Damping Configuration

Source: https://motion.dev/docs/glide

Demonstrates the bounceDamping option which controls the opposing force of the spring animation when boundaries are exceeded. Higher values reduce bounciness and create more controlled snap-back behavior.

```javascript
glide({ max: 100, bounceDamping: 30 })
```

--------------------------------

### useInView with Amount Option

Source: https://motion.dev/docs/vue-use-in-view

Control how much of an element must enter the viewport to be considered 'in view'. Accepts 'some', 'all', or a decimal between 0 and 1 representing the percentage threshold.

```vue
const isInView = useInView(domRef, { amount: "all" })
```

--------------------------------

### Troubleshooting Layout Animations with AnimatePresence and LayoutGroup (React)

Source: https://motion.dev/docs/react-animate-presence

When combining exit and layout animations, especially with `mode="sync"`, wrapping the animated group in `LayoutGroup` can resolve issues where components outside AnimatePresence don't correctly perform layout animations. This ensures proper coordination of layout changes.

```jsx
<LayoutGroup>
  <motion.ul layout>
    <AnimatePresence>
      {items.map(item => (
        <motion.li layout key={item.id} />
      ))}
    </AnimatePresence>
  </motion.ul>
</LayoutGroup>
```

--------------------------------

### Log Velocity Changes with useMotionValueEvent (React)

Source: https://motion.dev/docs/react-use-velocity

Illustrates how to use `useMotionValue` and `useVelocity` in a React component, and then log the latest velocity value to the console using `useMotionValueEvent` whenever the velocity changes. This is useful for debugging or triggering side effects based on velocity updates.

```javascript
import { useMotionValue, useVelocity } from "framer-motion"

function Component() {
  const x = useMotionValue(0)
  const xVelocity = useVelocity(x)

  useMotionValueEvent(xVelocity, "change", latest => {
    console.log("Velocity", latest)
  })
  
  return <motion.div style={{ x }} />
}
```

--------------------------------

### useReducedMotion Hook Import and Basic Usage

Source: https://motion.dev/docs/react-use-reduced-motion

Import and use the useReducedMotion hook from Motion library to detect Reduced Motion settings. The hook returns a boolean value that can be used to conditionally apply animations or alternative UI behaviors based on user accessibility preferences.

```javascript
import { useReducedMotion } from "motion/react"

const prefersReducedMotion = useReducedMotion()
```

--------------------------------

### Control Video Playback with usePageInView

Source: https://motion.dev/docs/react-use-page-in-view

Pause and resume video playback based on page visibility state using usePageInView with useRef and useEffect. When the page is hidden, the video pauses; when visible, it resumes playback.

```javascript
const videoRef = useRef(null)
const isInView = usePageInView()

useEffect(() => {
  const videoElement = videoRef.current
  if (!videoElement) return

  if (isInView) {
    videoElement.play()
  } else {
    videoElement.pause()
  }
}, [isInView])
```

--------------------------------

### Apply Tap Animations with `whileTap` in Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `whileTap` prop defines an animation state or variant label to apply when a tap/press gesture is active. It can be used to animate properties directly or trigger predefined variants for interactive elements.

```javascript
// As target
<motion.button whileTap={{ scale: 0.9 }} />
```

```javascript
// As variants
<motion.div whileTap="tapped" />
```

--------------------------------

### attrEffect with Aria and Data Attributes

Source: https://motion.dev/docs/attr-effect

Shows how attrEffect automatically converts camelCase attribute names to kebab-case for aria and data attributes. The resulting HTML element will have properly formatted aria-valuenow and data-value attributes.

```javascript
const value = motionValue("#fff")

attrEffect(counter, {
  ariaValuenow: value,
  dataValue: value
})

// <div aria-valuenow="#fff" data-value="#fff">
```

--------------------------------

### dragPropagation

Source: https://motion.dev/docs/react-motion-component

Allows drag gesture propagation to child components.

```APIDOC
## dragPropagation

### Description
Allows drag gesture propagation to child components.

### Type
`boolean`

### Default
`false`

### Usage Example
```jsx
<motion.div drag="x" dragPropagation />
```
```

--------------------------------

### Cancel attrEffect with Cleanup Function

Source: https://motion.dev/docs/attr-effect

Demonstrates how attrEffect returns a cleanup function that can be called to stop applying motion value changes to element attributes. Useful for cleanup in component lifecycles or when effects are no longer needed.

```javascript
const cx = motionValue(0)
const cy = motionValue(0)
const cancel = attrEffect("circle", { cx, cy })

cancel()
```

--------------------------------

### Animating the Scoped Element Directly with `useAnimate`

Source: https://motion.dev/docs/react-use-animate

This snippet shows how to animate the element that holds the `scope` ref itself. By passing `scope.current` as the target to the `animate` function, you can apply animations directly to the container element, such as changing its opacity over a specified duration.

```javascript
animate(scope.current, { opacity: 1 }, { duration: 1 })
```

--------------------------------

### Import EasingCurve from motion-studio

Source: https://motion.dev/docs/studio-sdk-easing-curve

Import the EasingCurve component from the motion-studio package to use it in your React application. This is the first step required to use the component.

```javascript
import { EasingCurve } from "motion-studio"
```

--------------------------------

### useInView with Custom Scrollable Container

Source: https://motion.dev/docs/vue-use-in-view

Configure useInView to track visibility within a custom scrollable parent element instead of the window viewport. Pass a computed ref with the root option pointing to the container element.

```vue
<script setup>
import { useInView } from 'motion-v'
import { computed } from 'vue'

const container = ref()
const boxRef = ref()
const isInView = useInView(boxRef, computed(() => ({ root: container.value })))
</script>

<template>
  <div ref="container" style="overflow: scroll">
    <div ref="boxRef" />
  </div>
</template>
```

--------------------------------

### Nested Exit Animations in Motion Components

Source: https://motion.dev/docs/react-animate-presence

Shows how nested motion components within an exiting component can each define their own exit animations. Child motion components fire their exit animations before the parent is removed from the DOM.

```jsx
function Slide({ img, description }) {
  return (
    <motion.div exit={{ opacity: 0 }}>
      <img src={img.src} />
      <motion.p exit={{ y: 10 }}>{description}</motion.p>
    </motion.div>
  )
}
```

--------------------------------

### Monitoring Motion Value Velocity Changes in Vue

Source: https://motion.dev/docs/vue-use-velocity

This Vue component demonstrates how to observe and react to changes in a motion value's velocity. It uses `useMotionValue` for an element's position, `useVelocity` to calculate its speed, and `useMotionValueEvent` to log the latest velocity value to the console whenever it updates.

```vue
<script setup>
import { useMotionValue, useVelocity, useMotionValueEvent } from 'motion-v'

const x = useMotionValue(0)
const xVelocity = useVelocity(x)

useMotionValueEvent(xVelocity, 'change', (latest) => {
  console.log('Velocity', latest)
})
</script>

<template>
  <Motion :style="{ x }" />
</template>
```

--------------------------------

### Slideshow Component with Key Changes

Source: https://motion.dev/docs/react-animate-presence

Implements a slideshow component using AnimatePresence where changing the image key triggers exit animation on the old image and entrance animation on the new image.

```jsx
export const Slideshow = ({ image }) => (
  <AnimatePresence>
    <motion.img
      key={image.src}
      src={image.src}
      initial={{ x: 300, opacity: 0 }}
      animate={{ x: 0, opacity: 1 }}
      exit={{ x: -300, opacity: 0 }}
    />
  </AnimatePresence>
)
```

--------------------------------

### Mapping Motion Value to Colors with `useTransform` (React)

Source: https://motion.dev/docs/react-use-transform

Demonstrates `useTransform`'s ability to map a numerical motion value to color values. As `x` changes from 0 to 100, the `backgroundColor` will interpolate smoothly between red and blue.

```javascript
const backgroundColor = useTransform(
  x,
  [0, 100],
  ["#f00", "#00f"]
)
```

--------------------------------

### Suggest Framer Motion 'whileInView' for Performance

Source: https://motion.dev/docs/animation-performance-audit

This snippet illustrates an anti-pattern improvement where an 'animate' prop with 'repeat: Infinity' is replaced by 'whileInView'. The audit suggests this change to ensure animations only run when visible in the viewport, conserving resources and improving overall performance, especially for long-running off-screen animations.

```jsx
<motion.div
  whileInView={keyframes}
  transition={{ repeat: Infinity }}
/>
```

--------------------------------

### Optimize Layout Animation Performance with `layoutDependency` in Motion.dev

Source: https://motion.dev/docs/vue-motion-component

Optimizes layout animation performance by controlling when measurements occur. Layout changes are only re-measured when the provided `layoutDependency` value changes, reducing unnecessary computations.

```html
<motion.nav layout :layoutDependency="isOpen" />
```

--------------------------------

### Configure Spring Stiffness Parameter

Source: https://motion.dev/docs/animate

Sets the stiffness of spring animations with a default value of 1. Higher stiffness values create more sudden, responsive movement. This parameter directly affects how quickly the spring responds to animation targets.

```javascript
animate(
  "section",
  { rotate: 180 },
  { type: "spring", stiffness: 50 }
)
```

--------------------------------

### CSS spring animation fallback for browser compatibility

Source: https://motion.dev/docs/css

Provide fallback transitions for browsers that don't support the linear() easing function by setting multiple transition declarations with different specificity levels. Use matching visualDuration for consistent animation feel.

```css
transition: filter 0.3s ease-out;
transition: filter ${spring(0.3)};
```

--------------------------------

### Dynamically Configure Reduced Motion in React with MotionConfig

Source: https://motion.dev/docs/react-accessibility

Shows how to dynamically set the `reducedMotion` prop on `MotionConfig` based on a user-defined setting (e.g., `userSetting`), allowing users to override the system's reduced motion preference for a specific site.

```javascript
<MotionConfig reducedMotion={userSetting}>
```

--------------------------------

### Partial Keyframes with WAAPI

Source: https://motion.dev/docs/improvements-to-the-web-animations-api-dx

Shows WAAPI's support for single keyframe definitions where the browser infers the initial keyframe from the element's current visual state. Motion automatically detects legacy browsers and generates initial keyframes using getComputedStyle().

```javascript
element.animate({ opacity: [0.2, 1] })
element.animate({ opacity: 1 })
```

--------------------------------

### Animate Flexbox Layout Changes in Vue

Source: https://motion.dev/docs/vue-layout-animations

Demonstrates animating changes to `justify-content` CSS property between `flex-start` and `flex-end` using the `layout` prop combined with conditional styling. The layout prop automatically handles the animation of previously non-animatable CSS values.

```vue
<motion.div
  layout
  :style="{ justifyContent: isOn ? 'flex-start' : 'flex-end' }"
/>
```

--------------------------------

### Motion Primitive with as-child Prop

Source: https://motion.dev/docs/vue-motion-component

Use the as-child prop to render a child element as the root element instead of creating a wrapper. This allows the Motion component to apply animations directly to the provided child element.

```vue
<script setup>
import { Motion } from "motion-v"
</script>
<template>
  <Motion as-child>
    <button>Click me</button>
  </Motion>
</template>
```

--------------------------------

### Compose Motion Values with useTransform Function

Source: https://motion.dev/docs/react-motion-value

Shows how to create a new motion value by composing one or more existing motion values using useTransform with a function. The function is called whenever any of the input motion values change.

```javascript
const y = useTransform(() => x.get() * 2)
```

--------------------------------

### AnimatePresence Custom Prop for Data Passing

Source: https://motion.dev/docs/react-animate-presence

Shows how to pass custom data through AnimatePresence using the custom prop. This data can be accessed by exiting components via usePresenceData hook.

```jsx
<AnimatePresence custom={swipeDirection}>
  <Slide key={activeSlideId} />
</AnimatePresence>
```

--------------------------------

### Create Motion component from custom DOM element

Source: https://motion.dev/docs/react-motion-component

Pass a string to motion.create() to create a motion-enabled custom DOM element. This will render the custom element into HTML with full animation capabilities.

```javascript
// Will render <custom-element /> into HTML
const MotionComponent = motion.create('custom-element')
```

--------------------------------

### Mapping Single Motion Value to Multiple Properties (Repetitive) (React)

Source: https://motion.dev/docs/react-use-transform

Shows a common pattern where a single input motion value (`offset`) is used to derive multiple output motion values (`opacity`, `scale`, `filter`) through separate `useTransform` calls. This approach can lead to repetition.

```javascript
const opacity = useTransform(offset, [100, 600], [1, 0.4])
const scale = useTransform(offset, [100, 600], [1, 0.6])
const filter = useTransform(offset, [100, 600], ["blur(0px)", "blur(10px)"])
```

--------------------------------

### Configure Viewport Tracking Options for Motion.dev Components

Source: https://motion.dev/docs/vue-motion-component

Configures how a `motion` component tracks its visibility within the viewport. Options like `once`, `root`, `margin`, and `amount` allow precise control over when intersection events are detected, enabling tailored animations based on scroll position.

```html
<motion.section
  :whileInView="{ opacity: 1 }"
  :inViewOptions="{ once: true }"
/>
```

--------------------------------

### layoutRoot - Fixed Position Layout Support

Source: https://motion.dev/docs/react-motion-component

Marks elements with position: fixed to account for page scroll in layout animations. Necessary for correct layout animation calculations within fixed-position containers.

```jsx
<motion.div layoutRoot style={{ position: "fixed" }}>
  <motion.div layout />
</motion.div>
```

--------------------------------

### Access press event details

Source: https://motion.dev/docs/press

Access the element and PointerEvent details in the press callback. The startEvent provides clientX and clientY coordinates of the press.

```javascript
press("div:nth-child(2)", (element, startEvent) => {
  console.log("Pressed", element)
  console.log("At", startEvent.clientX, startEvent.clientY)
})
```

--------------------------------

### EVENT /onUpdate

Source: https://motion.dev/docs/vue-motion-component

Callback triggered every frame any value on the `motion` component updates. It's provided a single argument with the latest values.

```APIDOC
## EVENT onUpdate\n\n### Description\nCallback triggered every frame any value on the `motion` component updates. It's provided a single argument with the latest values.\n\n### Type\nEvent\n\n### Arguments\n- **latest** (object) - The latest values of the component's motion properties.\n\n### Usage Example\n```vue\n<motion.article\n  :animate=\"{ opacity: 1 }\"\n  :@update=\"latest => console.log(latest.opacity)\"\n/>\n```\n
```

--------------------------------

### useTransform Multiple Output Values

Source: https://motion.dev/docs/vue-use-transform

Maps a single motion value to multiple output motion values in one call using a named map object. Reduces repetition when creating multiple derived values from the same source.

```JavaScript
const { opacity, scale, filter } = useTransform(offset, [100, 600], {
  opacity: [1, 0.4],
  scale: [1, 0.6],
  filter: ["blur(0px)", "blur(10px)"]
})
```

--------------------------------

### Complex CSS linear() easing curve with multiple control points

Source: https://motion.dev/docs/studio-generate-css

Extended CSS linear() easing function with numerous control points and percentage-based timing values. This demonstrates the full output of a generated spring animation with bounce effect, showing the complexity of maintainability when working directly with CSS linear() curves compared to Motion's declarative spring syntax.

```css
linear(
0, 0.009, 0.035 2.1%, 0.141, 0.281 6.7%, 0.723 12.9%, 0.938 16.7%, 1.017,
1.077, 1.121, 1.149 24.3%, 1.159, 1.163, 1.161, 1.154 29.9%, 1.129 32.8%,
1.051 39.6%, 1.017 43.1%, 0.991, 0.977 51%, 0.974 53.8%, 0.975 57.1%,
0.997 69.8%, 1.003 76.9%, 1.004 83.8%, 1
)
```

--------------------------------

### Spring animation with Tamagui

Source: https://motion.dev/docs/css

Use spring animations in Tamagui styled components by concatenating the spring() function output with string values in the transition property.

```javascript
export const RoundedSquare = styled(View, {
  transition: "opacity " + spring(0.5)
})
```

--------------------------------

### Subscribing to Motion Value changes and rendering with `frame.render` in JavaScript

Source: https://motion.dev/docs/motion-value

This snippet shows how to subscribe to a `motionValue`'s 'change' event and perform DOM updates within `frame.render`. This ensures that style changes are batched and applied efficiently on the next animation frame, optimizing performance.

```javascript
import { motionValue, frame } from "motion"

const color = motionValue("#fff")

color.on("change", latest => {
  frame.render(() => element.style.backgroundColor = latest)
})
```

--------------------------------

### Configure Initial Animation State

Source: https://motion.dev/docs/vue-motion-component

Set the initial visual state of a motion component using animation targets, variants, or arrays of variants. Set initial to false to disable enter animation and render with animate values instead.

```vue
<!-- Animation target -->
<motion.section :initial="{ opacity: 0, x: 0 }" />

<!-- Single variant -->
<motion.li initial="visible" />

<!-- Multiple variants -->
<motion.div :initial="['visible', 'active']" />

<!-- Disable enter animation -->
<motion.div :initial="false" :animate="{ opacity: 0 }" />
```

--------------------------------

### Apply an Imported Easing Function to a Progress Value

Source: https://motion.dev/docs/easing-functions

This snippet illustrates how to use an imported easing function by passing a `0`-`1` progress value to it. The function then returns an eased progress value, transforming the linear input into a non-linear output based on the easing curve.

```javascript
const eased = easeIn(0.75)
```

--------------------------------

### usePresenceData Hook for Custom Data

Source: https://motion.dev/docs/react-animate-presence

Demonstrates using the usePresenceData hook to access custom data passed through AnimatePresence's custom prop. Allows exiting components to receive updated data even after being removed from React tree.

```jsx
import { AnimatePresence, usePresenceData } from "motion/react"

function Slide() {
  const isPresent = useIsPresent()
  const direction = usePresenceData()

  return (
    <motion.div exit={{ opacity: 0 }}>
      {isPresent ? "Here!" : "Exiting " + direction}
    </motion.div>
  )
}
```

--------------------------------

### Fixing Exit Animations: Avoid `index` as `key` in Vue `v-for` with `AnimatePresence`

Source: https://motion.dev/docs/vue-animate-presence

This snippet demonstrates an incorrect pattern where `index` is used as a `key` within a `v-for` loop inside `AnimatePresence`. Using `index` can lead to incorrect exit animations when list items reorder, as the key no longer uniquely identifies the item.

```html
<AnimatePresence>
  <Component v-for="(item,index) in items" :key="index" />
</AnimatePresence>
```

--------------------------------

### complete() Method

Source: https://motion.dev/docs/animate

Immediately completes the animation by jumping to the end state. All animated values are set to their final target values.

```APIDOC
## complete() Method

### Description
Immediately completes the animation, running it to the end state.

### Method
- **complete()** - Jumps animation to final state

### Usage Example
```javascript
const animation = animate(element, { opacity: 0 })
animation.complete()
```
```

--------------------------------

### Animating individual transforms with Motion (CSS variables)

Source: https://motion.dev/docs/performance

This JavaScript code demonstrates animating individual `x` and `scale` properties on an element with the class `.box` using the Motion library. Motion achieves this by animating CSS variables under the hood. A key limitation is that animations using this method are currently not hardware accelerated, even though they apply to `transform` properties.

```javascript
animate(".box", { x: 100, scale: 2 })
```

--------------------------------

### Enforcing m Component Usage with LazyMotion strict Prop (React)

Source: https://motion.dev/docs/react-lazy-motion

This snippet demonstrates the use of the `strict` prop with `LazyMotion`. When set to `true`, `LazyMotion` will throw an error if a full `motion` component is used instead of the lightweight `m` component, helping to enforce bundle size optimizations.

```jsx
// This component will throw an error that explains using a motion component
// instead of the m component will break the benefits of code-splitting.
function Component() {
  return (
    <LazyMotion features={domAnimation} strict>
      <motion.div />
    </LazyMotion>
  )
}
```

--------------------------------

### Set Default Transition on a Motion Component (Vue)

Source: https://motion.dev/docs/vue-transitions

This snippet illustrates how to set a default transition directly on a `motion.div` component. This transition will apply to all animations within that specific component unless overridden by a more specific transition definition.

```vue
<motion.div
  :animate="{ x: 100 }"
  :transition="{ type: 'spring', stiffness: 100 }"
/>
```

--------------------------------

### AnimatePresence mode Prop

Source: https://motion.dev/docs/react-animate-presence

Defines how AnimatePresence handles the entering and exiting of children, with options for synchronous, waiting, or layout-aware animations.

```APIDOC
## mode

### Description
Decides how `AnimatePresence` handles entering and exiting children. Defaults to `"sync"`.

### Method
Component Prop

### Endpoint
AnimatePresence

### Parameters
#### Request Body
- **mode** (string) - Optional - Specifies the animation sequencing behavior. Can be `"sync"`, `"wait"`, or `"popLayout"`.

### Request Example
```jsx
<AnimatePresence mode="wait">
  {/* Children components */}
</AnimatePresence>
```

### Response
#### Success Response (N/A)
- This prop controls component behavior, not a direct API response.

#### Response Example
N/A

### Sub-modes
#### `sync`
In `"sync"` mode, elements animate in and out as soon as they're added/removed. This is the most basic (and default) mode - `AnimatePresence` takes no opinion on sequencing animations or layout. Therefore, if element layouts conflict (as in the above example), you can either implement your own solution (using `position: absolute` or similar), or try one of the other two `mode` options.

#### `wait`
In `"wait"` mode, the entering element will **wait** until the exiting child has animated out, before it animates in.
This is great for sequential animations, presenting users with one piece of information or one UI element at a time.
`wait` mode only supports one child at a time.
Try setting `ease: "easeIn"` (or similar) on the exit animation, and `ease: "easeOut"` on the enter animation for an overall `easeInOut` easing effect.

#### `popLayout`
Exiting elements will be "popped" out of the page layout, allowing surrounding elements to immediately reflow. Pairs especially well with the `layout` prop, so elements can animate to their new layout.

```jsx
<AnimatePresence mode="popLayout">
  {items.map(item => (
    <motion.li layout exit={{ opacity: 0 }} key={item.id} />
  ))}
</AnimatePresence>
```

When using `popLayout` mode, any immediate child of AnimatePresence that's a custom component **must** be wrapped in React's `forwardRef` function, forwarding the provided `ref` to the DOM node you wish to pop out of the layout.
```

--------------------------------

### Create accordion items with individual state management

Source: https://motion.dev/docs/react-layout-group

Defines an Item component that manages its own open/closed state and performs layout animations. Each item is a motion.div with a layout prop that animates when the isOpen state changes.

```jsx
function Item({ header, content }) {
  const [isOpen, setIsOpen] = useState(false)
  return (
    <motion.div
      layout
      onClick={() => setIsOpen(!isOpen)}
    >
      <motion.h2 layout>{header}</motion.h2>
      {isOpen ? content : null}
    </motion.div>
  )
}
```

--------------------------------

### Group Layout Animations with LayoutGroup

Source: https://motion.dev/docs/vue-layout-animations

Wraps multiple motion components in a `LayoutGroup` to synchronize layout animations across them. When one component re-renders and affects others' layout, all grouped components will animate together.

```vue
<script setup>
import { LayoutGroup } from "motion-v"
</script>

<template>
  <LayoutGroup>
    <Accordion />
    <Accordion />
  </LayoutGroup>
</template>
```

--------------------------------

### Configure Spring Damping Parameter

Source: https://motion.dev/docs/animate

Controls the strength of the opposing force in spring animations with a default value of 10. Setting damping to 0 causes the spring to oscillate indefinitely. Higher damping values reduce oscillation and settle animations faster.

```javascript
animate(
  "section",
  { rotate: 180 },
  { type: "spring", damping: 300 }
)
```

--------------------------------

### Animate MotionValue Strings with scrambleText

Source: https://motion.dev/docs/scramble-text

Illustrates how to integrate `scrambleText` with a `MotionValue<string>` to animate text changes. It includes subscribing to `MotionValue` changes to update the DOM element's text content, enabling dynamic text animations.

```javascript
import { scrambleText } from "motion-plus-dom"
import { motionValue } from "motion"

const text = motionValue("Hello world!")

// Subscribe to changes
text.on("change", (latest) => {
  document.querySelector("#title").textContent = latest
})

scrambleText(text, { duration: 1 })
```

--------------------------------

### useMotionValueEvent - Advanced Manual Subscription with Watch

Source: https://motion.dev/docs/vue-use-motion-value-event

Demonstrates advanced usage of the motion value's `on` method within a Vue watch for manual event subscription. Requires explicit unsubscription in the cleanup callback to prevent memory leaks when the component unmounts.

```vue
watch([x, y], (n, o, onCleanUp) => {
  const doSomething = () => {}
  
  const unsubX = x.on("change", doSomething)
  const unsubY = y.on("change", doSomething)
  
  onCleanUp(() => {
    unsubX()
    unsubY()
  })
}, {
  immediate: true
})
```

--------------------------------

### layout - Enable Layout Animations

Source: https://motion.dev/docs/react-motion-component

Enables automatic layout animations when component dimensions or position change. Can be boolean (true for full animation) or string ('position' or 'size') to animate only specific properties.

```jsx
<motion.div layout />
```

```jsx
<motion.img layout="position" />
```

--------------------------------

### Enable touch support with touch-action style

Source: https://motion.dev/docs/vue-use-drag-controls

Apply touch-action: none CSS style to the triggering element to ensure proper touch screen support. This prevents default browser touch behaviors and allows the drag controls to function correctly on touch devices.

```vue
<template>
  <div 
    @pointerdown="startDrag" 
    style="touch-action: none"
  />
</template>
```

--------------------------------

### Configure Damping for Spring Animation in Framer Motion

Source: https://motion.dev/docs/vue-transitions

Sets the strength of the opposing force in a spring animation. A higher value increases resistance, causing the animation to settle faster. If set to 0, the spring will oscillate indefinitely. Default is 10.

```Framer Motion
<motion.a
  :animate="{ rotate: 180 }"
  :transition="{ type: 'spring', damping: 300 }"
/>
```

--------------------------------

### Implementing a Border Workaround for Motion Animations

Source: https://motion.dev/docs/vue-layout-animations

Directly animating `border` can cause performance issues and visual stretching due to `1px` minimum rendering. A workaround is to simulate a border using a parent `motion.div` with `padding` and `borderRadius`, containing another `motion.div` for the inner content.

```JSX
<motion.div layout :style="{ borderRadius: '10px', padding: '5px' }">
  <motion.div layout "style="{ borderRadius: '5px' }" />
</motion.div>
```

--------------------------------

### AnimatePresence initial Prop

Source: https://motion.dev/docs/react-animate-presence

Controls whether initial animations are disabled for children present when AnimatePresence first renders.

```APIDOC
## initial

### Description
By passing `initial={false}`, `AnimatePresence` will disable any initial animations on children that are present when the component is first rendered.

### Method
Component Prop

### Endpoint
AnimatePresence

### Parameters
#### Request Body
- **initial** (boolean) - Optional - If `false`, disables initial animations for children present on first render.

### Request Example
```jsx
<AnimatePresence initial={false}>
  <Slide key={activeItem.id} />
</AnimatePresence>
```

### Response
#### Success Response (N/A)
- This prop controls component behavior, not a direct API response.

#### Response Example
N/A
```

--------------------------------

### Configure Power for Inertia Animation in Framer Motion

Source: https://motion.dev/docs/vue-transitions

Adjusts the 'power' of an inertia animation, which influences how far the target value is calculated. A higher power value results in a further calculated target. Default is 0.8.

```Framer Motion
<motion.div
  drag
  :dragTransition="{ power: 0.2 }"
/>
```

--------------------------------

### Define a basic callback in Motion.dev animation sequence

Source: https://motion.dev/docs/animate

Demonstrates how to insert a simple callback function into an animation sequence. The callback receives the latest progress value (0-1) for the segment duration.

```javascript
const sequence = [
  [(latest) => console.log(latest)]
]
```

--------------------------------

### Using `LazyMotion` `strict` prop to prevent `motion` component usage in Vue

Source: https://motion.dev/docs/vue-lazymotion

Explains the `strict` prop of `LazyMotion`, which, when set to `true`, throws an error if a full `motion` component is used instead of the lightweight `m` component within its scope. This helps ensure that the bundle size benefits of lazy-loading are not accidentally negated.

```html
<template>
    <LazyMotion :features="domAnimation" strict>
      <motion.div />
    </LazyMotion>
</template>
```

--------------------------------

### useIsPresence Hook for Presence State

Source: https://motion.dev/docs/react-animate-presence

Shows how to use the useIsPresence hook to access presence state within an AnimatePresence child component. Allows conditional rendering based on whether the component is present or exiting.

```jsx
import { useIsPresent } from "motion/react"

function Component() {
  const isPresent = useIsPresent()

  return isPresent ? "Here!" : "Exiting..."
}
```

--------------------------------

### Import motion component from framer-motion-3d

Source: https://motion.dev/docs/react-three-fiber

This line imports the `motion` object from the `framer-motion-3d` library. The `motion` object is used to create animated versions of React Three Fiber components, enabling declarative 3D animations.

```javascript
import { motion } from "framer-motion-3d"
```

--------------------------------

### Mapping Single Motion Value to Multiple Properties (Named Map) (React)

Source: https://motion.dev/docs/react-use-transform

Demonstrates a more efficient way to derive multiple motion values from a single input using `useTransform`'s named map feature. This reduces boilerplate compared to individual `useTransform` calls for each property.

```javascript
const { opacity, scale, filter } = useTransform(offset, [100, 600], {
  opacity: [1, 0.4],
  scale: [1, 0.6],
  filter: ["blur(0px)", "blur(10px)"],
})
```

--------------------------------

### Exit animations in list rendering with v-for

Source: https://motion.dev/docs/vue-animate-presence

AnimatePresence detects when list items are added or removed and applies exit animations to each item. Each item must have a unique key prop.

```vue
<AnimatePresence>
  <motion.li 
    v-for="item in items" 
    :key="item.id" 
    :exit="{ opacity: 1 }" 
    layout
  />
</AnimatePresence>
```

--------------------------------

### Control drag initiation with dragListener

Source: https://motion.dev/docs/react-motion-component

Determines whether the drag gesture is triggered by event listeners on the draggable element. When dragControls are provided and dragListener is set to false, dragging can only be initiated through the controls, not by pointer events on the element.

```JSX
<motion.div drag dragControls={dragControls} dragListener={false} />
```

--------------------------------

### Generate CSS spring transition with toString()

Source: https://motion.dev/docs/css

Use the spring() function with toString() method to generate CSS duration and easing values. The function accepts visualDuration and bounce parameters to create spring animations that can be embedded directly in CSS rules.

```javascript
transition: transform ${spring(0.5, 0.2)};

// Outputs:
// transition: transform 800ms linear(...)
```

--------------------------------

### Create Custom Motion Components

Source: https://motion.dev/docs/vue-motion-component

Convert any Vue component into a motion component using motion.create() function. This enables animation capabilities on custom components. Can also create custom DOM elements by passing strings. Avoid calling motion.create() in templates to prevent breaking animations.

```vue
const MotionComponent = motion.create(Component)

// Create custom DOM element
const MotionComponent = motion.create('custom-element')

// Forward motion props to component
motion.create(Component, { forwardMotionProps: true })
```

--------------------------------

### Accessing Element and Intersection Info in Callback (JavaScript)

Source: https://motion.dev/docs/inview

Details how the `inView` callback provides two arguments: the matched DOM `element` and an `IntersectionObserverEntry` object, which contains detailed information about the intersection event.

```javascript
inView("a", (element, info) => {
  console.log("The link ", element, " has entered the viewport")
})
```

--------------------------------

### Apply Hover Animations with whileHover

Source: https://motion.dev/docs/vue-motion-component

Define animation targets or variant labels to apply while hovering over a component. Can be used as a direct animation target object or reference a named variant. Automatically reverts when hover ends.

```vue
<!-- As target -->
<motion.button :whileHover="{ scale: 1.2 }" />

<!-- As variants -->
<motion.div whileHover="hovered" />
```

--------------------------------

### Immediately Completing an Animation (JavaScript)

Source: https://motion.dev/docs/animate

The `complete()` method instantly advances the animation to its final state. This is useful for quickly skipping to the end of an animation without waiting for its natural duration.

```javascript
animation.complete()
```

--------------------------------

### Configure `bounce` for spring animations in Motion.dev

Source: https://motion.dev/docs/animate

Illustrates setting the `bounce` option for `spring` type animations. This value (0-1) controls the bounciness, with higher values resulting in more pronounced bounce. It's overridden if physics-based options like `stiffness` are present.

```javascript
animate(
  "section",
  { rotateX: 90 },
  { type: "spring", bounce: 0.25 }
)
```

--------------------------------

### Update motion values to trigger style changes

Source: https://motion.dev/docs/style-effect

Update motion values using set() or animate() methods to trigger automatic style updates on the next animation frame. Multiple motion values can be updated independently.

```javascript
opacity.set(1)
animate(backgroundColor, "rgba(34, 255, 0, 1)")
```

--------------------------------

### `transform` with `clamp: false` for infinite mapping (JavaScript)

Source: https://motion.dev/docs/transform

This snippet showcases the use of the `clamp: false` option with `transform`, which allows the mapping function to extend infinitely beyond the defined input range. When `clamp` is set to `false`, input values outside the initial range will continue to be mapped proportionally rather than being capped at the output range's limits.

```javascript
const transformer = transform([0, 100], [0, 360], { clamp: false })

const rotation = transformer(200) // 720
```

--------------------------------

### Apply `mix` function with progress values in JavaScript

Source: https://motion.dev/docs/mix

Once initialized, the mixer function takes a progress value (typically `0`-`1`) to return an interpolated result. The `mix` function also gracefully handles progress values outside the `0`-`1` range, extrapolating the mixed value linearly.

```javascript
const mixComplex = mix("0px 0px #fff", "100px 100px #000")

mixComplex(0.5) // 50px 50px rgba(128, 128, 128, 1)

const mixNumber = mix(0, 100)

mixNumber(2) // 200
mixNumber(-1) // -100
```

--------------------------------

### Disable initial animations with initial prop

Source: https://motion.dev/docs/vue-animate-presence

Pass :initial="false" to AnimatePresence to disable initial animations on children that are present when the component first renders.

```vue
<AnimatePresence :initial="false">
  <Slide :key="activeItem.id" />
</AnimatePresence>
```

--------------------------------

### Motion Primitive Component with as Prop

Source: https://motion.dev/docs/vue-motion-component

Use the Motion primitive component to dynamically change the rendered element via the 'as' prop. This provides a Radix UI Primitives-like pattern for flexible component rendering in Vue.

```vue
<script setup>
import { Motion } from "motion-v"
</script>
<template>
  <Motion as="button">
    Click me
  </Motion>
</template>
```

--------------------------------

### Create SVG draw animation with `pathLength` using `svgEffect` (JavaScript)

Source: https://motion.dev/docs/svg-effect

`svgEffect` simplifies "draw"-style animations for SVG elements. This snippet demonstrates using `pathLength` as a `0`-`1` progress value to control how much of an SVG path is drawn, allowing for dynamic line drawing effects.

```JavaScript
const pathLength = motionValue(0.5)

svgEffect("circle", { pathLength }) // 0.5 = half path length
```

--------------------------------

### Applying Generated Tailwind CSS Spring Easing Utility Class

Source: https://motion.dev/docs/react-tailwind

This snippet demonstrates how to apply a custom CSS spring easing, generated by Motion for AI and defined in the Tailwind theme, to an element. The `ease-spring-soft` utility class is used to control the animation's timing function.

```html
<div className="transition-transform duration-700 ease-spring-soft">
```

--------------------------------

### Motion component with server-side rendering

Source: https://motion.dev/docs/react-motion-component

Motion components are fully compatible with server-side rendering (SSR). Set initial={false} to disable enter animations and render the component with values from the animate prop. The server will output the correct initial state in the generated HTML.

```javascript
// Server will output `translateX(100px)`
<motion.div initial={false} animate={{ x: 100 }} />
```

--------------------------------

### Spring Animations with Motion

Source: https://motion.dev/docs/improvements-to-the-web-animations-api-dx

Motion supports spring-based animations by compiling springs into linear() easing with computed durations in animateStyle, or pre-calculating keyframes for physics-based animations in the animate function.

```JavaScript
import { animate } from "motion/dom"
import { spring } from "motion"

animate(
  "li",
  { transform: "translateX(100px)" },
  { type: spring, stiffness: 400 }
)
```

--------------------------------

### Handle onDrag callback with position and velocity info

Source: https://motion.dev/docs/react-motion-component

Callback function that fires when a drag gesture is recognized. Receives the PointerEvent and an info object containing point (device/page relative), delta (distance since last event), offset (distance from original event), and velocity data.

```JSX
function onDrag(event, info) {
  console.log(info.point.x, info.point.y)
}

<motion.div drag onDrag={onDrag} />
```

--------------------------------

### Updating `springValue` Targets with the `.set()` Method in JavaScript

Source: https://motion.dev/docs/spring-value

Following initialization, this snippet shows how to programmatically change the target value of a `springValue` instance using its `.set()` method. Calling `.set()` on `scaleX` and `rotate` will cause them to animate from their current value to the new target with a spring effect.

```javascript
scaleX.set(1)
rotate.set("2turn")
```

--------------------------------

### Configure Spring Animation Bounce in Motion (Vue)

Source: https://motion.dev/docs/vue-transitions

This snippet shows how to set the `bounce` property for a spring animation to control its bounciness. A value of `0` results in no bounce, while `1` creates an extremely bouncy effect. Note that `bounce` is overridden if `stiffness`, `damping`, or `mass` are also set.

```vue
<motion.div
  :animate="{ rotateX: 90 }"
  :transition="{ type: 'spring', bounce: 0.25 }"
/>
```

--------------------------------

### Define Ticker Items Array - React

Source: https://motion.dev/docs/react-ticker

Demonstrates how to create an array of React nodes to pass to the Ticker component. Items can be JSX elements, strings, or numbers that will be animated in the ticker.

```jsx
const items = [
  <span>One</span>,
  <span>Two</span>,
  <span>Three</span>
]

return <Ticker items={items} />
```

--------------------------------

### AnimatePresence onExitComplete Prop

Source: https://motion.dev/docs/react-animate-presence

A callback function that fires when all exiting child components have finished their animation.

```APIDOC
## onExitComplete

### Description
Fires when all exiting nodes have completed animating out.

### Method
Component Prop

### Endpoint
AnimatePresence

### Parameters
#### Request Body
- **onExitComplete** (function) - Optional - A callback function executed after all children have completed their exit animations.

### Request Example
```jsx
<AnimatePresence onExitComplete={() => console.log("All exits complete")}>
  {/* Children components */}
</AnimatePresence>
```

### Response
#### Success Response (N/A)
- This prop controls component behavior, not a direct API response.

#### Response Example
N/A
```

--------------------------------

### useReducedMotion with Conditional Animation in React

Source: https://motion.dev/docs/react-use-reduced-motion

Demonstrates using useReducedMotion to conditionally modify animation properties in a Motion component. When Reduced Motion is enabled, the hook returns true and animations are replaced with simpler alternatives (e.g., x-axis movement replaced with opacity changes). The component re-renders automatically when the setting changes.

```javascript
export function Sidebar({ isOpen }) {
  const shouldReduceMotion = useReducedMotion()
  const closedX = shouldReduceMotion ? 0 : "-100%"
  
  return (
    <motion.div animate={{
      opacity: isOpen ? 1 : 0,
      x: isOpen ? 0 : closedX
    }} />
  )
}
```

--------------------------------

### Animating Scale Based on Drag Velocity in Vue

Source: https://motion.dev/docs/vue-use-velocity

This Vue component demonstrates how to dynamically adjust an element's scale based on its drag velocity. It uses `useMotionValue` for position, `useVelocity` to derive velocity, and `useTransform` to map velocity values to a scale range, creating an interactive visual effect.

```vue
<script setup>
const x = useMotionValue(0)
const xVelocity = useVelocity(x)
const scale = useTransform(
  xVelocity,
  [-3000, 0, 3000],
  [2, 1, 2],
  { clamp: false }
)
</script>

<template>
  <Motion drag="x" :style="{ x, scale }" />
</template>
```

--------------------------------

### Import `svgEffect` from 'motion' (JavaScript)

Source: https://motion.dev/docs/svg-effect

This code snippet illustrates the standard way to import the `svgEffect` function into your JavaScript or TypeScript project. It is essential to import this function from the 'motion' library before it can be used to animate SVG elements.

```JavaScript
import { svgEffect } from "motion"
```

--------------------------------

### Configure Animation Repeat Delay Parameter

Source: https://motion.dev/docs/animate

Sets the wait duration between animation repetitions in seconds with a default value of 0. Not available in animate mini. Allows precise control over timing between repeated animation cycles.

```javascript
animate(
  element,
  { backgroundColor: "#fff" },
  { repeat: 1, repeatDelay: 1 }
)
```

--------------------------------

### Basic Motion component usage

Source: https://motion.dev/docs/react-motion-component

Use motion components as you would normal HTML/SVG elements. Motion components are prefixed with 'motion.' (e.g., motion.div, motion.circle) and support standard React props like className. They can be enhanced with animation props for declarative animations.

```javascript
<motion.div className="box" />
```

--------------------------------

### Staggering Animations with `stagger`

Source: https://motion.dev/docs/animate

Apply staggered delays to animations across multiple elements using the `stagger` function, creating sequential animation effects.

```APIDOC
## FUNCTION `stagger`

### Description
The `stagger` function is used with the `delay` option to apply incremental delays to a group of animated elements, making them animate in sequence rather than all at once.

### Function Signature
`stagger(interval, options)`

### Parameters
#### Arguments for `stagger`
- **interval** (number) - Required - The delay interval in seconds between each staggered element.
- **options** (object) - Optional - Additional options for staggering (not detailed in source, but common for stagger functions).

### Example Usage
```javascript
import { stagger, animate } from "motion"

animate(".item", { x: 300 }, { delay: stagger(0.1) })
```

### Effect/Output
Each element matching `.item` will animate with a `0.1` second delay relative to the previous element, creating a staggered animation effect.
```
// First .item animates
// 0.1s later, second .item animates
// 0.1s later, third .item animates
// ...
```
```

--------------------------------

### Define Easing Functions by Name or Bezier Curve in Motion

Source: https://motion.dev/docs/easing-functions

This snippet demonstrates how to specify easing functions within Motion's `animate` or `motion` components. Easing can be defined either by using a predefined name like 'easeIn' for common curves or by providing a custom Bezier curve as an array of control points for precise control.

```javascript
// Named easing
ease: "easeIn"

// Bezier curve
ease: [0.39, 0.24, 0.3, 1]
```

--------------------------------

### delay() - Animation Frame Synchronized Delay

Source: https://motion.dev/docs/delay

The delay function provides a setTimeout alternative that fires callbacks synchronized with Motion's animation frame loop. It returns a cancellation function and integrates with Motion's read/write batching system for optimal performance.

```APIDOC
## delay()

### Description
A setTimeout alternative that's locked to Motion's animation frame loop. This synchronizes callbacks with other animations and avoids the overhead of setting many setTimeout instances.

### Method
Function

### Signature
```
delay(callback: Function, duration: number): Function
```

### Parameters
#### Function Parameters
- **callback** (Function) - Required - The function to execute after the specified duration
- **duration** (number) - Required - Duration in seconds before the callback fires

### Return Value
- **cancel** (Function) - A function that when called will cancel the scheduled delay and prevent the callback from firing

### Request Example
```javascript
import { delay } from "motion"

// Basic delay
delay(() => console.log("one second!"), 1)

// Delay with cancellation
const cancel = delay(callback, 0.25)
cancel() // callback will never fire
```

### Response Example
```javascript
// Callback fires after 1 second on the animation frame
// Output: "one second!"

// Cancel function prevents execution
const cancel = delay(() => console.log("test"), 1)
cancel() // No output
```

### Behavior
- Callback fires on the first step of Motion's animation loop (the `read` step)
- Enables batching of reads and writes with the rest of the animation loop
- Can be combined with `frame.render()` for coordinated rendering

### Integration Example
```javascript
import { delay, frame } from "motion"

delay(() => {
  const { left } = element.getBoundingClientRect()

  // Will render later during this animation frame
  frame.render(() => {
    element.style.left = `${left * 2}px`
  })
}, 1)
```

### Notes
- Duration is measured in seconds (not milliseconds like setTimeout)
- Integrates with Motion's animation frame loop for better performance
- Useful for synchronizing multiple animations and callbacks
- Reduces overhead compared to multiple setTimeout calls
```

--------------------------------

### play() Method

Source: https://motion.dev/docs/animate

Plays an animation. If paused, it resumes from the current time. If finished, it restarts from the beginning.

```APIDOC
## play() Method

### Description
Plays an animation.

### Behavior
- If an animation is **paused**, it will resume from its current `time`
- If an animation has **finished**, it will restart from the beginning

### Method
- **play()** - Resumes or restarts animation playback

### Usage Examples
```javascript
// Resume from paused state at 1 second
animation.pause()
animation.time = 1
animation.play()

// Restart from beginning after completion
await animation
animation.play()
```
```

--------------------------------

### Update Element Height in JavaScript

Source: https://motion.dev/docs/performance

This JavaScript snippet demonstrates directly setting an element's height using `element.style.height`. This operation typically triggers a full browser re-render cycle (layout, paint, composite), making it less suitable for smooth animations due to its performance impact.

```javascript
element.style.height = "500px"
```

--------------------------------

### Apply Focus Animations with whileFocus

Source: https://motion.dev/docs/vue-motion-component

Define animation targets or variant labels to apply while a component has focus. Can be used as a direct animation target object or reference a named variant. Useful for form inputs and interactive elements.

```vue
<!-- As target -->
<motion.button :whileFocus="{ outline: 'dashed #000' }" />

<!-- As variants -->
<motion.div whileFocus="focused" />
```

--------------------------------

### Set Inline Transition on Motion Component Hover (Vue)

Source: https://motion.dev/docs/vue-transitions

This snippet shows how to define a transition directly within an animation prop, such as `:whileHover`, for specific interactive states. The transition defined here will only apply when the component is hovered, allowing for fine-grained control over state-based animations.

```vue
<motion.div
  :whileHover="{
    scale: 1.1,
    transition: { duration: 0.2 }
  }"
/>
```

--------------------------------

### Jump Motion Value to Break Animation Continuity

Source: https://motion.dev/docs/react-motion-value

Shows how to use the jump() method to set a motion value to a new state while breaking continuity from previous values. This resets velocity to 0, ends active animations, and ignores attached effects like springs.

```javascript
const x = useSpring(0)
x.jump(10)
x.getVelocity() // 0
```

--------------------------------

### Spring animation with Astro CSS variables

Source: https://motion.dev/docs/css

Define spring animations as CSS variables in Astro using the define:vars directive, then reference them in CSS using var() function for dynamic spring transitions.

```javascript
<style define:vars={{ spring: spring(0.2, 0) }}>
  span {
    transition: transform var(--spring);
  }
</style>
```

--------------------------------

### Namespace multiple TabRow components with LayoutGroup and id prop

Source: https://motion.dev/docs/react-layout-group

Wraps a TabRow in LayoutGroup with a unique id prop to namespace the layoutId scope. This allows multiple independent TabRow instances on the same page without layout animation conflicts.

```jsx
function TabRow({ id, items }) {
  return (
    <LayoutGroup id={id}>
      {items.map(item => <Tab {...item} />)}
    </LayoutGroup>
  )
}
```

--------------------------------

### Import Cursor component from motion-plus

Source: https://motion.dev/docs/cursor

Import the Cursor component from the motion-plus React package. This makes the component available for use in your React application.

```javascript
import { Cursor } from "motion-plus/react"
```

--------------------------------

### Configure Bounce Stiffness for Inertia Animation Constraints in Framer Motion

Source: https://motion.dev/docs/vue-transitions

Affects the stiffness of the spring animation when the value hits `min` or `max` constraints in an inertia animation. Higher values will create a more sudden bounce effect. Default is 500.

```Framer Motion
<motion.div
  drag
  :dragTransition="{
    min: 0,
    max: 100,
    bounceStiffness: 100
  }"
/>
```

--------------------------------

### Configure Exit Animation for Motion Component

Source: https://motion.dev/docs/vue-motion-component

Define animation targets that execute when a motion component is removed from the tree. Can be set as animation targets or variants. The component must be a direct child of AnimatePresence for exit animations to work properly.

```vue
<AnimatePresence>
    <ul v-if="isVisible"  key="list">
      <motion.li :exit="{ opacity: 0 }" />
    </ul>
</AnimatePresence>
```

--------------------------------

### Handling Animation Completion with then() (JavaScript)

Source: https://motion.dev/docs/animate

The animation object provides a Promise-like `then()` API, allowing you to execute code when the animation finishes. This can be used with `async/await` or traditional Promise callbacks to chain actions after an animation completes.

```javascript
const animation = animate(element, { opacity: 0 })

// Async/await
await animation
console.log("Animation complete")

// Promise
animation.then(() => {
  console.log("Animation complete")
})
```

--------------------------------

### Configure dragConstraints with pixel values

Source: https://motion.dev/docs/react-motion-component

Set drag constraints using an object with optional top, left, right, and bottom pixel values to limit the draggable area. Alternatively, pass a ref to another element to use its bounding box as constraints.

```JSX
<motion.div
  drag="x"
  dragConstraints={{ left: 0, right: 300 }}
/>
```

```JSX
const MyComponent = () => {
  const constraintsRef = useRef(null)

  return (
     <motion.div ref={constraintsRef}>
         <motion.div drag dragConstraints={constraintsRef} />
     </motion.div>
  )
}
```

--------------------------------

### Exit animations with v-show directive

Source: https://motion.dev/docs/vue-animate-presence

AnimatePresence works with v-show to trigger exit animations when visibility changes, providing an alternative to v-if for conditional rendering.

```vue
<AnimatePresence>
  <Modal v-show="show" key="modal" />
</AnimatePresence>
```

--------------------------------

### Apply Text Scrambling to DOM Elements or Selectors with motion-plus-dom

Source: https://motion.dev/docs/scramble-text

Shows how to use `scrambleText` from `motion-plus-dom` with both a CSS selector and a direct DOM element reference. This allows flexible targeting of text content for animation, providing options for different integration scenarios.

```javascript
import { scrambleText } from "motion-plus-dom"

// With selector
scrambleText("#title", { duration: 1 })

// With element reference
const element = document.querySelector(".text")
scrambleText(element, { duration: 1 })
```

--------------------------------

### Stagger animations for multiple elements using Motion.dev

Source: https://motion.dev/docs/animate

Illustrates how to apply a staggered delay to animations for multiple elements. The `stagger` function is passed to the `delay` option of the `animate` function, creating a sequential animation effect.

```javascript
import { stagger, animate } from "motion"

animate(".item", { x: 300 }, { delay: stagger(0.1) })
```

--------------------------------

### AnimatePresence for Exit Animations

Source: https://motion.dev/docs/vue-layout-animations

Wraps a conditionally rendered motion element to keep it in the DOM until its exit animation completes. Useful for animating elements back to their origin layout before removal.

```vue
<AnimatePresence>
  <motion.div v-if="isOpen" layoutId="modal" />
</AnimatePresence>
```

--------------------------------

### Create custom Motion component

Source: https://motion.dev/docs/react-motion-component

Convert any React component into a motion component using motion.create(). The component must forward a ref to the element you want to animate. In React 18, use forwardRef; in React 19, pass ref via props. Avoid calling motion.create() inside render functions to prevent breaking animations.

```javascript
const MotionComponent = motion.create(Component)
```

--------------------------------

### Import useDragControls from Motion React

Source: https://motion.dev/docs/react-use-drag-controls

Import the useDragControls hook from the Motion React library to enable programmatic drag control functionality in your React components.

```javascript
import { useDragControls } from "motion/react"
```

--------------------------------

### Basic animate() Function Usage - JavaScript

Source: https://motion.dev/docs/animate

Demonstrates the fundamental usage of the animate() function to animate HTML elements and SVG styles. The function accepts an element or CSS selector, animation properties object, and optional configuration options.

```javascript
animate("li", { opacity: 0 })
```

--------------------------------

### Motion component variants configuration

Source: https://motion.dev/docs/react-motion-component

Define reusable animation states as a variants object with named animation targets and optional transitions. Variants enable declarative, maintainable animations that can be referenced by name in animation props like initial, animate, and exit.

```javascript
const variants = {
  active: {
      backgroundColor: "#f00"
  },
  inactive: {
    backgroundColor: "#fff",
    transition: { duration: 2 }
  }
}

return (
  <motion.div
    variants={variants}
    animate={isActive ? "active" : "inactive"}
  />
)
```

--------------------------------

### Track another motion value with useSpring

Source: https://motion.dev/docs/react-use-spring

Create a useSpring that automatically animates towards the latest value of another motion value. The source motion value must be a number or unit-type string, enabling reactive spring animations.

```javascript
const x = useMotionValue(0)
const y = useSpring(x)
```

--------------------------------

### Handle Pan Gesture with `onPan` Callback in Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `onPan` callback function fires continuously when a pan gesture is recognized on the element. It provides the `PointerEvent` and an `info` object containing `point`, `delta`, `offset`, and `velocity` for detailed pan tracking. For touch input, ensure `touch-action` CSS is set appropriately.

```javascript
function onPan(event, info) {
  console.log(info.point.x, info.point.y)
}

<motion.div onPan={onPan} />
```

--------------------------------

### AnimatePresence with Conditional Rendering

Source: https://motion.dev/docs/react-animate-presence

Demonstrates AnimatePresence detecting when a Modal component is removed from the React tree due to mounting/remounting. The key prop is required for AnimatePresence to track component presence.

```jsx
<AnimatePresence>
  {show && <Modal key="modal" />}
</AnimatePresence>
```

--------------------------------

### ScrambleText Custom Character Presets in JavaScript

Source: https://motion.dev/docs/react-scramble-text

Defines several JavaScript constants, each containing a different array or string of characters. These presets can be used with the `chars` prop to achieve various visual effects, such as symbols, blocks, hex, or emojis.

```javascript
const symbols = "!@#$%^&*()_+-=[]{}|;:,.<>?/~`░▒▓█▀▄■□▪▫●○◆◇◈◊※†‡"
const blocks = "█▓▒░"
const binary = "01"
const hex = "0123456789ABCDEF"
const katakana = "アイウエオカキクケコサシスセソタチツテトナニヌネノハヒフヘホマミムメモヤユヨラリルレロワヲン"
const faces =  ["😀", "😃", "😄", "😁", "😆", "😅", "🤣", "😂", "🙂", "😊"]
const dots = "⠁⠂⠃⠄⠅⠆⠇⠈⠉⠊⠋⠌⠍⠎⠏"
```

--------------------------------

### Set Stiffness for Spring Animation in Framer Motion

Source: https://motion.dev/docs/vue-transitions

Controls the stiffness of the spring in an animation. Higher stiffness values create more sudden and rapid movement. Default is 1.

```Framer Motion
<motion.section
  animate={{ rotate: 180 }}
  transition={{ type: 'spring', stiffness: 50 }}
/>
```

--------------------------------

### Animate HTML and SVG Elements - JavaScript

Source: https://motion.dev/docs/animate

Demonstrates animating HTML and SVG elements using both direct element references and CSS selectors. Supports passing duration and other animation options as configuration parameters.

```javascript
// Element(s)
const box = document.getElementById("box")

animate(box, { opacity: 0 }, { duration: 0.5 })

// CSS selectors
animate("div", { opacity: 0 }, { duration: 0.5 })
```

--------------------------------

### Jumping a Motion Value to a new state and resetting velocity in JavaScript

Source: https://motion.dev/docs/motion-value

This code demonstrates the `jump` method, which immediately sets a `motionValue` to a new state, effectively breaking continuity. It also resets the velocity to `0` and stops any active animations, providing a clean transition point.

```javascript
animate(x, 100)

x.jump(10)
x.getVelocity() // 0
```

--------------------------------

### Apply Focus Animations with `whileFocus` in Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `whileFocus` prop defines an animation state or variant label to apply when the component is focused. It can be used to animate properties directly or trigger predefined variants for accessibility and interactive elements.

```javascript
// As target
<motion.button whileFocus={{ outline: "dashed #000" }} />
```

```javascript
// As variants
<motion.div whileFocus="focused" />
```

--------------------------------

### Motion component with animation props

Source: https://motion.dev/docs/react-motion-component

Enhance motion components with powerful animation APIs including animate for value changes, whileInView for viewport-triggered animations, layout for layout change animations, and style with independent transforms. These props enable declarative, performant animations without React re-renders.

```javascript
<motion.div
  className="box"
  // Animate when this value changes:
  animate={{ scale: 2 }}
  // Fade in when the element enters the viewport:
  whileInView={{ opacity: 1 }}
  // Animate the component when its layout changes:
  layout
  // Style now supports indepedent transforms:
  style={{ x: 100 }}
/>
```

--------------------------------

### Coordinate spring animations with other transitions

Source: https://motion.dev/docs/css

Combine spring animations with other CSS transitions using visualDuration to ensure animations appear to take similar time despite different actual durations. The visualDuration defines time to reach target, excluding bounce effects.

```css
transition:
  opacity 0.5s ease-out,
  transform ${spring(0.5, 0.2)};
```

--------------------------------

### Apply Press Animations with whilePress

Source: https://motion.dev/docs/vue-motion-component

Define animation targets or variant labels to apply while pressing a component. Can be used as a direct animation target object or reference a named variant. Automatically reverts when press ends.

```vue
<!-- As target -->
<motion.button :whilePress="{ scale: 0.9 }" />

<!-- As variants -->
<motion.div whilePress="tapped" />
```

--------------------------------

### onViewportEnter - Viewport Entry Callback

Source: https://motion.dev/docs/react-motion-component

Callback function triggered when an element enters the viewport. Receives IntersectionObserverEntry object containing intersection event details like isIntersecting status.

```jsx
<motion.div onViewportEnter={(entry) => console.log(entry.isIntersecting)} />
```

--------------------------------

### layoutDependency - Optimize Layout Measurements

Source: https://motion.dev/docs/react-motion-component

Reduces performance overhead by limiting layout measurements to when this dependency value changes. By default, measurements occur every render; this prop allows selective measurement triggering.

```jsx
<motion.nav layout layoutDependency={isOpen} />
```

--------------------------------

### Nested exit animations on child motion components

Source: https://motion.dev/docs/vue-animate-presence

Any motion components within an exiting component will fire animations defined on their exit props before the parent component is removed from the DOM.

```vue
<template>
  <motion.div :exit="{ opacity: 0 }">
    <img :src="img.src" />
    <motion.p :exit="{ y: 10 }">{{description}}</motion.p>
  </motion.div>
</template>
```

--------------------------------

### Configure Animation Update Callback with onUpdate

Source: https://motion.dev/docs/animate

Provides a callback function that receives the latest animation values during each frame. Currently works only for single value animations. Useful for synchronizing external logic with animation progress or debugging animation values.

```javascript
animate("#fff", "#000", {
  duration: 2,
  onUpdate: latest => console.log(latest)
})
```

--------------------------------

### Create and attach drag controls to motion component

Source: https://motion.dev/docs/react-use-drag-controls

Initialize drag controls using useDragControls hook and pass them to a motion.div component with the drag prop. This creates a draggable element that can be controlled programmatically.

```javascript
const controls = useDragControls()

return <motion.div drag dragControls={controls} />
```

--------------------------------

### Typewriter Dynamic Content Backspace by Word in React

Source: https://motion.dev/docs/react-typewriter

Configures the `Typewriter` component to backspace content word by word when its `children` prop changes. This provides a more natural animation for updating dynamic text.

```jsx
<Typewriter backspace="word">{text}</Typewriter>
```

--------------------------------

### Import useDragControls from Motion Vue

Source: https://motion.dev/docs/vue-use-drag-controls

Import the useDragControls composable and motion component from the motion-v package. This is the first step to enable manual drag control functionality in your Vue application.

```javascript
import { useDragControls } from "motion-v"
```

--------------------------------

### Glide Configuration with Decay Parameter

Source: https://motion.dev/docs/glide

Shows how to adjust the decay time constant (in seconds) which controls velocity decay rate. Higher decay values result in longer animations with more gradual deceleration and a lighter feel.

```javascript
glide({ decay: 0.5 })
```

--------------------------------

### Applying Motion Values to DOM elements with `styleEffect` in JavaScript

Source: https://motion.dev/docs/motion-value

This snippet illustrates how `motionValue` instances can be linked to DOM element styles using `styleEffect`. Changes to `x` and `opacity` Motion Values will automatically update the corresponding CSS properties for all `<li>` elements on the next animation frame, enabling declarative and performant animations.

```javascript
const x = motionValue(0)
const opacity = motionValue(1)

styleEffect("li", { x, opacity })

x.set(100) // Will apply to all <li> elements on the next frame
animate(opacity, 0) // Will animate all <li> opacity
```

--------------------------------

### Animate Single Values with onUpdate Callback - JavaScript

Source: https://motion.dev/docs/animate

Demonstrates animating numeric and color values by passing 'to' and 'from' values. The onUpdate callback receives the latest animated value during each frame.

```javascript
// Numbers
animate(0, 100, {
  onUpdate: latest => console.log(latest)
})

// Colors
animate("#fff", "#000", {
  duration: 2,
  onUpdate: latest => console.log(latest)
})
```

--------------------------------

### Animation `type` - Mini `animate`

Source: https://motion.dev/docs/animate

Configure the animation type for `motion/mini`'s `animate` function, supporting default keyframes or `spring` animations.

```APIDOC
## OPTION `type` - Mini `animate`

### Description
The `type` option in `motion/mini`'s `animate` function determines the animation engine to use. It supports default keyframe animations or `spring` physics-based animations.

### Parameters
#### Options Object Properties
- **type** (function) - Optional - Specifies the animation type. Can be `spring` from `motion`.
- **stiffness** (number) - Optional - (For `spring` type) Defines the stiffness of the spring.

### Example Usage
```javascript
import { animate } from "motion/mini"
import { spring } from "motion"

animate(
  element,
  { transform: "translateX(100px)" },
  { type: spring, stiffness: 300 }
)
```

###
```

--------------------------------

### Handle Tap Event with `onTap` Callback in Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `onTap` callback function is invoked when a pointer stops pressing the component and was released inside the component's bounds. It provides the triggering `PointerEvent` object, useful for click-like interactions.

```javascript
<motion.div onTap={(event) => console.log(event)} />
```

--------------------------------

### Conditional Layout Animation with Width Changes

Source: https://motion.dev/docs/vue-layout-animations

Animates width changes based on conditional state using the `layout` prop. CSS changes are applied immediately via the `style` prop, while the `layout` prop handles the animation automatically.

```vue
<motion.div layout :style="{ width: isOpen ? '80vw' : 0 }" />
```

--------------------------------

### Add transitions between EasingCurve animations

Source: https://motion.dev/docs/studio-sdk-easing-curve

Enable smooth animations when switching between different easing curves by providing a transition prop with duration and other animation settings. This is useful for preset curve animations but may feel unresponsive during direct curve editing.

```javascript
<EasingCurve curve={curve} transition={{ duration: 0.3 }} />
```

--------------------------------

### Combine Steps Easing with Another Easing Function for Distribution

Source: https://motion.dev/docs/easing-functions

This snippet shows an advanced usage of the `steps` easing function where its linear distribution is modified by first passing the progress through another easing function, such as `circInOut`. This allows for non-linear distribution of the discrete steps.

```javascript
const easing = steps(4)

easing(circInOut(0.2))
```

--------------------------------

### Configure Spring Mass Parameter

Source: https://motion.dev/docs/animate

Sets the mass of the moving object in spring animations with a default value of 1. Higher mass values result in more lethargic, slower movement. Lower mass values create lighter, more responsive animations.

```javascript
animate(
  "feTurbulence",
  { baseFrequency: 0.5 },
  { type: "spring", mass: 0.5 }
)
```

--------------------------------

### Server-Side Rendering with Motion Component

Source: https://motion.dev/docs/vue-motion-component

Motion components are fully compatible with server-side rendering. Set initial prop to false to disable enter animation and render initial state from animate prop. The server will output the correct CSS transforms in the generated HTML.

```vue
<!-- Server will output `translateX(100px)` -->
<motion.div :initial="false" :animate="{ x: 100 }" />
```

--------------------------------

### Create Motion Value with useMotionValue Hook

Source: https://motion.dev/docs/vue-motion-value

Initialize a motion value with an initial numeric or string state using the useMotionValue hook. This creates a composable, signal-like value that tracks animation state and can be passed to motion components via the style prop.

```vue
<script setup>
import { motion, useMotionValue } from "motion-v"
const x = useMotionValue(0)
</script>

<template>
<motion.div :style="{ x }" />
</template>
```

```javascript
import { useMotionValue } from "motion-v"

const x = useMotionValue(0)
```

--------------------------------

### PROPERTY /style

Source: https://motion.dev/docs/vue-motion-component

The `style` property extends the normal Vue DOM `style` prop with support for motion values and independent transforms.

```APIDOC
## PROPERTY style\n\n### Description\nThe normal Vue DOM `style` prop, with added support for motion values and independent transforms.\n\n### Type\nProperty\n\n### Parameters\n- **style** (object) - Required - A style object, which can include motion values (e.g., `x`, `rotate`) and standard CSS properties.\n\n### Usage Example\n```vue\n<script setup>\n  const x = useMotionValue(30)\n</script>\n\n<template>\n  <motion.div :style=\"{ x, rotate: 90, originX: 0.5 }\" />\n</template>\n```\n
```

--------------------------------

### Animate element while in viewport with whileInView

Source: https://motion.dev/docs/vue-motion-component

Apply target animations or variant labels to elements while they are visible in the viewport. Can be used as a target object with animation properties or as a string referencing a variant name.

```vue
<motion.div :whileInView="{ opacity: 1 }" />
```

```vue
<motion.div whileInView="visible" />
```

--------------------------------

### Customize Scramble Characters in scrambleText

Source: https://motion.dev/docs/scramble-text

Demonstrates how to provide custom character sets for the `scrambleText` animation, including binary, symbols, and multi-byte emoji characters using an array. This allows for unique visual effects beyond the default alphanumeric set.

```javascript
// Binary effect
scrambleText(element, { chars: "01", duration: 1 })

// Symbols
scrambleText(element, {
  chars: "!@#$%^&*()_+-=[]{}|;:,.<>?/~`░▒▓█▀▄■□▪▫●○◆◇◈◊※†‡"
})

// Emoji (use array for multi-byte characters)
scrambleText(element, {
  chars: ["😀", "😃", "😄", "😁", "😆", "😅"]
})
```

--------------------------------

### Initialize `mix` function for various value types in JavaScript

Source: https://motion.dev/docs/mix

The `mix` function from the Motion library creates an interpolator between two values. It supports a wide range of data types including numbers, colors (RGBA, HSLA), complex strings, and nested arrays or objects. RGB color mixing uses a linear RGB space for accurate results, avoiding common brightness issues.

```javascript
const mixer = mix(0, 100)
mixer(0.5) // 50

import { mix } from "motion"
const mixNumber = mix(0, 100)
const mixColor = mix("#000", "#FFF")
const mixObject = mix(
  { a: "0px", b: 10 },
  { a: "20px", b: 0 }
)
```

--------------------------------

### Handle Element Entering Viewport in Motion.dev

Source: https://motion.dev/docs/vue-motion-component

Defines a callback function that executes when a `motion` component enters the viewport. It receives an `IntersectionObserverEntry` object, providing detailed information about the intersection event for custom logic.

```html
<motion.div @viewportEnter="(entry) => console.log(entry.isIntersecting)" />
```

--------------------------------

### Motion component animate prop with variants

Source: https://motion.dev/docs/react-motion-component

Use variant names as strings or arrays with the animate prop to apply predefined animation states. This enables declarative, reusable animations that can be easily toggled or sequenced.

```javascript
<motion.li animate="visible" />

<motion.div initial="hidden" animate={["visible", "active"]} />
```

--------------------------------

### Handle Pan End Events

Source: https://motion.dev/docs/vue-motion-component

The onPanEnd callback fires when a pan gesture ends. Receives the triggering PointerEvent and info object containing delta, point, offset, and velocity properties.

```vue
<motion.div @panEnd="(event, info) => console.log(info.delta.x)" />
```

--------------------------------

### dragControls

Source: https://motion.dev/docs/react-motion-component

Enables initiating a drag gesture from a different component than the draggable one using the `useDragControls` hook.

```APIDOC
## dragControls

### Description
Allows initiating dragging from a different component than the draggable one. By creating `dragControls` using the `useDragControls` hook, we can pass this into the draggable component's `dragControls` prop. It exposes a `start` method that can start dragging from pointer events on other components.

### Type
`DragControls`

### Usage Example
```jsx
const dragControls = useDragControls()

function startDrag(event) {
  dragControls.start(event, { snapToCursor: true })
}

return (
  <>
    <div onPointerDown={startDrag} />
    <motion.div drag="x" dragControls={dragControls} />
  </>
)
```

### Notes
When setting `dragControls`, it is possible to disable the draggable element as the initiator by setting `dragListener={false}`.
```

--------------------------------

### Implement lightweight hover gesture recognition with `hover()` function in React

Source: https://motion.dev/docs/react-hover-animation

For lightweight hover detection without importing the full `motion` component, the `hover()` function can be used. Integrated with React's `useEffect` and `useRef`, it allows you to attach hover listeners to any DOM element. The function returns a cleanup function, making it easy to manage event listeners within a component's lifecycle.

```javascript
import { hover } from "motion"
import { useRef, useEffect } from "react"

function Component() {
  const ref = useRef(null)

  useEffect(() => {
    return hover(ref.current, () => {
      console.log("on hover start")

      return () => console.log("on hover end")
    })
  }, [])

  return <button ref={ref} />
}
```

--------------------------------

### Create tabbed interface with shared layoutId animations

Source: https://motion.dev/docs/react-layout-group

Implements a Tab component that renders a motion.div with layoutId="underline" when selected. The layoutId prop enables shared layout animations across tabs, allowing smooth underline transitions between selected tabs.

```jsx
function Tab({ label, isSelected }) {
  return (
    <li>
      {label}
      {isSelected
        ? <motion.div layoutId="underline" />
        : null}
    </li>  
  )
}

function TabRow({ items }) {
  return items.map(item => <Tab {...item} />)
}
```

--------------------------------

### Configure Animation Repeat Parameter

Source: https://motion.dev/docs/animate

Sets the number of times to repeat an animation with a default value of 0. Set to Infinity for perpetual animation. Works in conjunction with repeatType and repeatDelay to control animation looping behavior.

```javascript
animate(
  element,
  { backgroundColor: "#fff" },
  { repeat: Infinity, duration: 2 }
)
```

--------------------------------

### Import and Basic Usage of Motion Component

Source: https://motion.dev/docs/vue-motion-component

Import the motion component from motion-v library and use it as a normal Vue component with enhanced animation capabilities. The motion component works with any HTML or SVG element (e.g., motion.div, motion.circle) and supports animation props like animate, whileInView, and layout.

```vue
import { motion } from "motion-v"

<motion.div class="box" />

<motion.div
  class="box"
  :animate="{ scale: 2 }"
  :whileInView="{ opacity: 1 }"
  layout
  :style="{ x: 100 }"
/>
```

--------------------------------

### Configure hover with once option

Source: https://motion.dev/docs/hover

Set the once option to true to fire the gesture only once per element. Default is false for continuous hover detection.

```javascript
hover(element, callback, { once: true })
```

--------------------------------

### Handle Pan End Event with `onPanEnd` Callback in Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `onPanEnd` callback function fires when a pan gesture concludes on the element. It provides the triggering `PointerEvent` and an `info` object with final gesture details, useful for completing pan-related actions.

```javascript
<motion.div onPanEnd={(event, info) => console.log(info.delta.x)} />
```

--------------------------------

### Setting a Motion Value's state in JavaScript

Source: https://motion.dev/docs/motion-value

This snippet demonstrates how to imperatively update the state of a `motionValue` using its `set` method. This directly changes the value without animation, triggering any 'change' event listeners.

```javascript
x.set(100)
```

--------------------------------

### Configure Animate Target for Motion Component

Source: https://motion.dev/docs/vue-motion-component

Define animation targets that the motion component animates to on enter and on update. Can be specified as animation targets with property values or as variant names, supporting single or multiple variants.

```vue
<!-- Animation target -->
<motion.div
  :initial="{ boxShadow: '0px 0px #000' }"
  :animate="{ boxShadow: '10px 10px #000' }"
/>

<!-- Single variant -->
<motion.li animate="visible" />

<!-- Multiple variants -->
<motion.div initial="hidden" :animate="['visible', 'active']" />
```

--------------------------------

### Reschedule Animation Sequence Segments - JavaScript

Source: https://motion.dev/docs/animate

Demonstrates how to control when segments play in an animation sequence using the 'at' option. Supports absolute time, relative time, or label-based scheduling.

```javascript
const sequence = [
  ["ul", { opacity: 1 }],
  ["li", { x: [-100, 0] }, { at: 1 }]
]

animate(sequence)
```

--------------------------------

### Fixing Layout Animations: Wrap with `LayoutGroup` for `mode="sync"` in Vue

Source: https://motion.dev/docs/vue-animate-presence

When mixing layout and exit animations with `mode="sync"`, components outside `AnimatePresence` might not animate correctly. Wrapping the group in `LayoutGroup` ensures all components coordinate their layout animations properly.

```html
<LayoutGroup>
  <motion.ul layout>
    <AnimatePresence>
        <motion.li v-for="item in items" layout :key="item.id" />
    </AnimatePresence>
  </motion.ul>
</LayoutGroup>
```

--------------------------------

### Import Motion component in React

Source: https://motion.dev/docs/react-motion-component

Import the motion component from the Motion library for use in React applications. Supports both standard React and React Server Components (Next.js). The motion component provides access to animation APIs and gesture handlers.

```javascript
// React
import { motion } from "motion/react"

// React Server Components (Next.js etc)
import * as motion from "motion/react-client"
```

--------------------------------

### useInView with Margin Option

Source: https://motion.dev/docs/vue-use-in-view

Adjust the detection area by adding margin around the viewport. Accepts CSS-style margin values (top/right/bottom/left) to expand or contract the detection boundary.

```vue
const isInView = useInView(domRef, {
  margin: "0px 100px -50px 0px"
})
```

--------------------------------

### Namespace multiple TabRow components with LayoutGroup and id prop

Source: https://motion.dev/docs/vue-layout-group

Shows how to use LayoutGroup with an id prop to namespace layoutId animations across multiple TabRow instances on the same page. This prevents layoutId conflicts when rendering multiple independent tab groups.

```vue
<!-- TabRow -->
<template>
  <LayoutGroup :id="id">
    <Tab v-for="item in items" :key="item.id" v-bind="item"/>
  </LayoutGroup>
</template>
```

--------------------------------

### Apply easing to `mix` function progress in JavaScript

Source: https://motion.dev/docs/mix

To achieve non-linear interpolation, an easing function can be applied to the progress value before passing it to the mixer. This allows for custom animation curves, such as `easeInOut`, to control the rate of change of the mixed value.

```javascript
import { mix, easeInOut } from "motion"

const mixNumber = mix(0, 100)

mixNumber(easeInOut(0.75))
```

--------------------------------

### Scope Animation Performance Audit to Specific Types

Source: https://motion.dev/docs/animation-performance-audit

This command demonstrates how to interact with the Motion+ Animation Performance Audit tool to scope an audit to specific types of animations or APIs. By providing a natural language query, users can direct the AI to focus on particular animation categories, such as 'scroll animations', for a more targeted performance analysis.

```cli
Can you perform a /motion-audit of all scroll animations
```

--------------------------------

### animate() - Timeline Sequences

Source: https://motion.dev/docs/animate

Create complex animation sequences with multiple elements and values playing in sequence or at specific times. Supports scheduling, transitions, and default settings.

```APIDOC
## animate() - Timeline Sequences

### Description
Create complex animation sequences with multiple animate definitions playing in sequence or at specific times. Available in the hybrid version.

### Syntax
```javascript
const sequence = [
  [target, properties, options?],
  [target, properties, options?]
]

animate(sequence, globalOptions?)
```

### Sequence Definition
Each segment is an array containing:
- **target** (Element | string | object | MotionValue) - Animation target
- **properties** (object | number) - Target animation values
- **options** (object) - Optional segment-specific animation options

### Request Example

#### Basic Sequence
```javascript
const sequence = [
  ["ul", { opacity: 1 }, { duration: 0.5 }],
  ["li", 100, { ease: "easeInOut" }]
]

animate(sequence)
```

### Scheduling Options

#### Absolute Time
```javascript
const sequence = [
  ["ul", { opacity: 1 }],
  ["li", { x: [-100, 0] }, { at: 1 }]
]
```

#### Relative Time
```javascript
{ at: "+0.5" }  // 0.5 seconds after previous
```

#### Label Reference
```javascript
{ at: "labelName" }
```

### Segment Transitions
Each segment accepts all animate options except `repeatDelay` and `repeatType`:

#### Uniform Duration
```javascript
const sequence = [
  ["ul", { opacity: 1 }, { duration: 1 }]
]
```

#### Per-Value Transitions
```javascript
const sequence = [
  [
    "ul",
    { opacity: 1, x: 100 },
    { duration: 1, x: { duration: 2 } }
  ]
]
```

#### Transition Types
Both `type: "keyframes"` and `type: "spring"` are supported.

### Global Sequence Options

#### Manual Duration
```javascript
animate(sequence, { duration: 10, repeat: 2 })
```

#### Default Transition
```javascript
animate(sequence, {
  defaultTransition: { duration: 0.2 }
})
```

### Mixed Subjects
```javascript
const color = motionValue("rgba(255, 0, 0, 1)")
const box = new THREE.BoxGeometry()

const sequence = [
  ["li", { x: 100 }],
  [box.position, { y: 10 }],
  [color, "#444"]
]

animate(sequence)
```

### Notes
- Segments play one after another by default
- Use `at` option to change timing
- Mix HTML, SVG, motion values, and objects in same sequence
- Sequence durations are automatically calculated
```

--------------------------------

### Use modifyTarget for Inertia Animation Snapping in Framer Motion

Source: https://motion.dev/docs/vue-transitions

A function that allows modification of the automatically calculated target value for an inertia animation. This is useful for implementing snap-to-grid or similar functionalities by returning a new target. The function receives the original target as an argument.

```Framer Motion
<motion.div
  drag
  // dragTransition always type: inertia
  :dragTransition="{
    power: 0,
    // Snap calculated target to nearest 50 pixels
    modifyTarget: target => Math.round(target / 50) * 50
  }"
/>
```

--------------------------------

### Fixing Exit Animations: Conditionally Render Child within `AnimatePresence` in Vue

Source: https://motion.dev/docs/vue-animate-presence

This snippet demonstrates the correct approach for conditional rendering with `AnimatePresence`. By placing the `v-if` on the child component, `AnimatePresence` remains mounted and can effectively manage the exit animations.

```html
<AnimatePresence>
  <Component v-if="isVisible" />
</AnimatePresence>
```

--------------------------------

### Mix Multiple Animation Subjects in Sequences - JavaScript

Source: https://motion.dev/docs/animate

Demonstrates animating multiple types of subjects in a single sequence, including HTML elements, motion values, and JavaScript objects like Three.js geometries.

```javascript
const color = motionValue("rgba(255, 0, 0, 1)")
const box = new THREE.BoxGeometry()

const sequence = [
  ["li", { x: 100 }],
  [box.position, { y: 10 }],
  [color, "#444"]
]

animate(sequence)
```

--------------------------------

### Animating percentage-based transform with Motion (potential non-acceleration)

Source: https://motion.dev/docs/performance

This JavaScript code snippet demonstrates animating an element's `transform` property using a percentage-based `translateX` value with the Motion library. It highlights a past browser-specific limitation where Chrome, until recently, would not hardware accelerate such percentage-based transforms, even though `transform` is generally considered performant. This emphasizes the variability in hardware acceleration across browsers and conditions.

```javascript
animate(element, { transform: "translateX(100%)" })
```

--------------------------------

### Demonstrating Default Clamping Behavior in mapValue (JavaScript)

Source: https://motion.dev/docs/map-value

This snippet shows `mapValue`'s default behavior where the output value is clamped to the specified range. If the input motion value exceeds the input range, the output is capped at the corresponding end of the output range, preventing extrapolation.

```javascript
const progress = motionValue(3)
const double = mapValue(progress, [0, 1], [0, 2])

double.get() // progress clamped to 1, outputs 2
```

--------------------------------

### Finished Promise Polyfill

Source: https://motion.dev/docs/improvements-to-the-web-animations-api-dx

Motion polyfills the animation.finished Promise for browsers that don't support this newer WAAPI spec feature, enabling consistent async/await and Promise-based animation completion handling.

```JavaScript
import { animate } from "motion/dom"

const animation = animate("#box", { opacity: 0 })

// Async/await
await animation

// Promise
animation.then(() => {})
```

--------------------------------

### Configure Spring Rest Speed Parameter

Source: https://motion.dev/docs/animate

Sets the threshold speed (in units per second) for animation completion with a default value of 0.1. Animation ends when absolute speed drops below this value and delta is smaller than restDelta, allowing precise control over when spring animations settle.

```javascript
animate(
  ".my-element",
  { rotate: 180 },
  { type: "spring", restSpeed: 2 }
)
```

--------------------------------

### Create tab underline with shared layoutId in Motion Vue

Source: https://motion.dev/docs/vue-layout-group

Demonstrates using the layoutId prop to create a shared layout animation across multiple Tab components. Each tab conditionally renders a motion.div with layoutId="underline" that animates between selected tabs.

```vue
<!-- Tab -->
<template>
  <li>
      {{label}}
      <motion.div v-if="isSelected" layoutId="underline" />
    </li> 
</template>

<!-- TabRow -->
<template>
  <Tab v-for="item in items" :key="item.id" v-bind="item"/>
</template>
```

--------------------------------

### useAnimationFrame Hook

Source: https://motion.dev/docs/vue-use-animation-frame

The useAnimationFrame composable executes a callback function on every animation frame. It provides two timing arguments: the total elapsed time since the callback was first called, and the delta time since the last frame. This is useful for creating smooth, frame-based animations.

```APIDOC
## useAnimationFrame

### Description
Runs a callback function once every animation frame, providing timing information for frame-based animations.

### Method
Composable Function

### Import
```javascript
import { useAnimationFrame } from 'motion-v'
```

### Syntax
```javascript
useAnimationFrame((time, delta) => {
  // Animation logic here
})
```

### Parameters
#### Callback Function Arguments
- **time** (number) - Required - The total duration of time in milliseconds since the callback was first called
- **delta** (number) - Required - The total duration of time in milliseconds since the last animation frame

### Usage Example
```javascript
<script setup>
import { useAnimationFrame } from 'motion-v'
import { ref } from 'vue'

const domRef = ref()

useAnimationFrame((time, delta) => {
  domRef.value.style.transform = `rotateY(${time}deg)`
})
</script>

<template>
  <div :ref="domRef" />
</template>
```

### Simple Example
```javascript
useAnimationFrame((time) => {
  domRef.value.style.transform = `rotateY(${time}deg)`
})
```

### Use Cases
- Creating smooth rotation animations
- Implementing frame-based motion effects
- Building custom animation sequences
- Synchronizing animations with browser refresh rate

### Notes
- The callback executes synchronously with the browser's animation frame
- Time values are cumulative from the initial callback invocation
- Delta provides frame-to-frame timing for frame-rate independent calculations
```

--------------------------------

### PROPERTY /variants

Source: https://motion.dev/docs/vue-motion-component

The `variants` property defines animation states for the component, allowing for state-based animations.

```APIDOC
## PROPERTY variants\n\n### Description\nThe variants for this component.\n\n### Type\nProperty\n\n### Parameters\n- **variants** (object) - Required - An object where keys are variant names and values are style objects, optionally including `transition` properties.\n\n### Usage Example\n```vue\n<script setup>\n  const variants = {\n    active: {\n        backgroundColor: \"#f00\"\n    },\n    inactive: {\n      backgroundColor: \"#fff\",\n      transition: { duration: 2 }\n    }\n  }\n</script>\n\n<template>  \n  <motion.div\n    :variants=\"variants\"\n    :animate=\"isActive ? 'active' : 'inactive'\"\n  />\n</template>\n```\n
```

--------------------------------

### Implement Hover Gesture with `whileHover` and Events in Vue

Source: https://motion.dev/docs/vue-gestures

This snippet shows how to detect hover events on a `motion.a` component. It uses `whileHover` for animation and `@hoverStart`, `@hoverEnd` event listeners to trigger custom logic when the pointer enters or leaves the component, distinct from standard mouse events.

```html
<motion.a
  :whileHover="{ scale: 1.2 }"
  @hoverStart="event => {}"
  @hoverEnd="event => {}"
/>
```

--------------------------------

### Conditionally render Cursor component

Source: https://motion.dev/docs/cursor

Conditionally render the Cursor component based on a state variable. When the condition is false, the component is removed and the browser's default cursor is restored.

```jsx
{isCursorVisible ? <Cursor /> : null}
```

--------------------------------

### attrEffect - Apply Motion Values to Element Attributes

Source: https://motion.dev/docs/attr-effect

attrEffect applies the output of motion values to the attributes of one or more elements. When motion values update, the element will re-render once per frame during the render step of the frameloop. It automatically handles casing for aria and data attributes, converting camelCase to kebab-case.

```APIDOC
## attrEffect

### Description
Applies the output of motion values to the attributes of one or more elements. When these motion values update, the element will re-render once per frame during the render step of the frameloop.

### Import
```javascript
import { attrEffect } from "motion"
```

### Syntax
```javascript
attrEffect(element, attributeMap)
```

### Parameters
#### element (required)
- **Type**: Element | Element[] | string (CSS selector)
- **Description**: A single element, array of elements, or CSS selector string targeting the element(s) to apply attributes to

#### attributeMap (required)
- **Type**: Object
- **Description**: A map of attribute names to motion values. Keys are attribute names, values are motion values to apply

### Return Value
- **Type**: Function
- **Description**: A cleanup function that, when called, stops applying changes to the motion values to the element

### Usage Examples

#### Basic Usage
```javascript
const width = motionValue(100)
attrEffect("rect", { width })
```

#### With CSS Selector
```javascript
const progress = motionValue(0.5)
attrEffect("#progress", { "data-progress": progress })
```

#### Aria and Data Attributes (Auto Casing)
```javascript
const value = motionValue("#fff")
attrEffect(counter, {
  ariaValuenow: value,
  dataValue: value
})
// Renders as: <div aria-valuenow="#fff" data-value="#fff">
```

#### Updating Motion Values
```javascript
const progress = motionValue(0.5)
attrEffect("#progress", { "data-progress": progress })

progress.set(1)
animate(progress, 1)
```

#### Multiple Elements
```javascript
const cx = motionValue(0)
const cy = motionValue(0)
attrEffect("circle", { cx, cy })
```

### Features
- Automatically handles casing for `aria` and `data` attributes, converting camelCase to kebab-case
- Dynamically sets attributes via their JavaScript setter for improved type-safety and performance
- Supports any motion value, including those defined by `mapValue` and `transformValue`
- Each motion value can be applied to any number of attributes on any number of elements

### Cleanup
```javascript
const cx = motionValue(0)
const cy = motionValue(0)
const cancel = attrEffect("circle", { cx, cy })

// Stop applying changes
cancel()
```
```

--------------------------------

### AnimatePresence Propagate Prop for Exit Animations

Source: https://motion.dev/docs/react-animate-presence

Demonstrates using the propagate prop set to true on nested AnimatePresence. This allows exit animations on inner children to fire when the outer AnimatePresence removes them.

```jsx
<AnimatePresence>
  {show ? (
    <motion.section exit={{ opacity: 0 }}>
      <AnimatePresence propagate>
        {/*
          * When `show` becomes `false`, exit animations
          * on these children **will** fire.
          */}
        {children}
      </AnimatePresence>
    </motion.section>
  ) : null}
</AnimatePresence>
```

--------------------------------

### Pass Custom Data to Dynamic Variants in Motion.dev

Source: https://motion.dev/docs/vue-motion-component

Provides a way to pass arbitrary data to dynamic variant functions. This allows for highly flexible and data-driven animation definitions, enabling variants to adapt their behavior based on runtime values.

```vue
<script setup>  
  const variants = {
    visible: (custom) => ({
      opacity: 1,
      transition: { delay: custom * 0.2 }
    })
  }
</script>

<template>
  <motion.ul animate="visible">
    <motion.li :custom="0" :variants="variants" />
    <motion.li :custom="1" :variants="variants" />
    <motion.li :custom="2" :variants="variants" />
  </motion.ul>
</template>
```

--------------------------------

### Conditional Shared Layout Animation with layoutId

Source: https://motion.dev/docs/vue-layout-animations

Demonstrates conditional rendering of a motion element with `layoutId` for shared layout animations. When the element is added, it animates from the previous element's position; when removed, it can be kept in the DOM using AnimatePresence.

```vue
<motion.div v-if="isSelected" layoutId="underline" />
```

--------------------------------

### Apply motion values to element styles with styleEffect

Source: https://motion.dev/docs/style-effect

Apply motion values to element styles using styleEffect by passing a CSS selector and an object mapping style properties to motion values. The element will re-render on each animation frame when motion values update.

```javascript
const opacity = motionValue(0.5)
const backgroundColor = motionValue("#00f")

styleEffect("div", { opacity, backgroundColor })
```

--------------------------------

### Apply Hover Animations with `whileHover` in Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `whileHover` prop defines an animation state or variant label to apply when a hover gesture is active. It can be used to animate properties directly or trigger predefined variants for interactive elements.

```javascript
// As target
<motion.button whileHover={{ scale: 1.2 }} />
```

```javascript
// As variants
<motion.div whileHover="hovered" />
```

--------------------------------

### Basic AnimateNumber Component Usage in Vue

Source: https://motion.dev/docs/vue-animate-number

This snippet demonstrates the fundamental way to use the `AnimateNumber` component within a Vue application. It binds a numeric value, typically a reactive data property like `count`, to the component to display an animated number. This is the core usage for creating dynamic number animations such as countdowns or engagement bars.

```html
<AnimateNumber :value="count"/>
```

--------------------------------

### Set SVG attributes using `attr` prefix with `svgEffect` (JavaScript)

Source: https://motion.dev/docs/svg-effect

By default, `svgEffect` applies valid styles via `.style`. This snippet shows how to explicitly set an SVG attribute (like `width`) using the `attr` prefix (e.g., `attrWidth`) when there's a direct attribute equivalent, allowing precise control over SVG properties.

```JavaScript
const width = motionValue(400)

svgEffect("rect", { attrWidth: width })
```

--------------------------------

### Configure EasingCurve layout with positioning props

Source: https://motion.dev/docs/studio-sdk-easing-curve

Set the size and position of the EasingCurve component using width, height, top, and left props measured in pixels. It is recommended to use equal width and height values for a square aspect ratio.

```javascript
<EasingCurve
  curve={curve}
  width={100}
  height={100}
  top={20}
/>
```

--------------------------------

### Watch useInView State Changes in Vue

Source: https://motion.dev/docs/vue-use-in-view

Use Vue's watch function to execute side effects when the isInView state changes. Useful for triggering animations, analytics, or other callbacks based on element visibility.

```vue
<script setup>
watch(isInView, (inView) => {
  console.log('Element is in view: ', inView)
})
</script>
```

--------------------------------

### Enable dragPropagation to child components

Source: https://motion.dev/docs/react-motion-component

Allows drag gestures to propagate from parent to child components. By default (false), drag gestures are contained to the component they are initiated on.

```JSX
<motion.div drag="x" dragPropagation />
```

--------------------------------

### Forward Motion props to custom component

Source: https://motion.dev/docs/react-motion-component

Enable motion props (like animate, whileHover, etc.) to be forwarded to custom components by setting forwardMotionProps config to true. By default, motion props are filtered out of the props passed to the component.

```javascript
motion.create(Component, { forwardMotionProps: true })
```

--------------------------------

### React Server Components spring animation

Source: https://motion.dev/docs/css

Set spring animations via the style prop in React Server Components for server-side execution with no runtime overhead. Supports both inline styles and style tags for defining spring transitions.

```javascript
<div style={{ transition: "all " + spring() }}>
```

```javascript
<style>{`
  button:hover {
    transition: transform ${spring(0.8, 0)};
    transform: scale(1.2);
  }
`}</style>
```

--------------------------------

### Custom Easing Functions with Motion

Source: https://motion.dev/docs/improvements-to-the-web-animations-api-dx

Motion extends WAAPI's limited easing functions by supporting custom easing functions through automatic linear() CSS easing generation. It automatically generates appropriate easing definitions for modern browsers with fallbacks for older browsers.

```JavaScript
import { animate } from "motion/dom"

animate(
  "li",
  { opacity: 1 },
  { ease: mirrorEasing(Math.sin) }
)
```

--------------------------------

### Enable strict mode to prevent motion component usage

Source: https://motion.dev/docs/react-reduce-bundle-size

Set the `strict` prop on LazyMotion to enforce use of the `m` component instead of the full `motion` component. When strict mode is enabled, including a `motion` component anywhere within LazyMotion will throw an error with a reminder to use `m` instead, preventing accidental bundle size increases.

```javascript
function App() {
  // This will throw!
  return (
    <LazyMotion strict>
      <motion.div />
    </LazyMotion>
  )
}
```

--------------------------------

### Animate Independent Transforms with Different Options

Source: https://motion.dev/docs/improvements-to-the-web-animations-api-dx

Demonstrates Motion's support for animating individual transform properties with different animation options. Each transform property can have its own duration, repeat count, and other animation parameters.

```javascript
animate(
  element,
  { x: 50, scaleX: 2 },
  { x: { duration: 2 }, scaleX: { repeat: 1 } }
)
```

--------------------------------

### Motion component animate prop with animation target

Source: https://motion.dev/docs/react-motion-component

Define target values to animate to on component enter and update using an animation target object. The animate prop can reference specific CSS properties and their target values for smooth transitions.

```javascript
<motion.div
  initial={{ boxShadow: "0px 0px #000" }}
  animate={{ boxShadow: "10px 10px #000" }}
/>
```

--------------------------------

### Enable Layout Animations for Radix Tabs with Motion Vue

Source: https://motion.dev/docs/vue-radix

This snippet shows how to enable layout animations for a Radix Tabs component. By using `v-model` to manage the active tab state and wrapping the `Tabs.Root` (with `as-child`) in a `motion.div` with the `layout` prop, Motion can automatically animate layout changes when the tab switches.

```Vue
<script setup>
const tab = ref('account')
</script>

<template>
  <Tabs.Root 
    v-model="tab" 
    as-child
  >
    <motion.div layout>

```

--------------------------------

### Override animation options on a per-value basis in Motion.dev

Source: https://motion.dev/docs/animate

Explains how to provide named transitions to override global animation options for specific properties. This allows for fine-grained control, such as setting a different duration or easing for individual animated values.

```javascript
animate(
  element,
  { x: 100, rotate: 0 },
  {
    duration: 1,
    rotate: { duration: 0.5, ease: "easeOut" }
  }
)
```

--------------------------------

### Create CSS filter from motionValue in JavaScript

Source: https://motion.dev/docs/transform-value

This snippet demonstrates how to use `transformValue` to create a CSS filter string dynamically from a `motionValue`. It shows how to apply the derived filter to an image element using `styleEffect`.

```javascript
const blur = motionValue(0)
const filter = transformValue(() => `blur(${blur.get()}px)`)

styleEffect("img", { filter })
```

--------------------------------

### animate() - Basic HTML & SVG Animation

Source: https://motion.dev/docs/animate

Animate HTML and SVG elements by passing element references or CSS selectors with target properties and optional animation options. Both mini and hybrid versions support this core functionality.

```APIDOC
## animate() - HTML & SVG Elements

### Description
Animate HTML and SVG styles using element references or CSS selectors. Supports opacity, colors, dimensions, and all standard CSS properties.

### Syntax
```javascript
animate(target, properties, options?)
```

### Parameters
- **target** (Element | string) - Required - DOM element or CSS selector string
- **properties** (object) - Required - Object containing target animation values
- **options** (object) - Optional - Animation configuration (duration, delay, ease, etc.)

### Request Examples

#### Animate by Element Reference
```javascript
const box = document.getElementById("box")
animate(box, { opacity: 0 }, { duration: 0.5 })
```

#### Animate by CSS Selector
```javascript
animate("div", { opacity: 0 }, { duration: 0.5 })
animate("li", { opacity: 0 })
```

### Response
Returns an animation controller that can be used to manage playback.

### Import
```javascript
// Hybrid version (18kb)
import { animate } from "motion"

// Mini version (2.3kb)
import { animate } from "motion/mini"
```
```

--------------------------------

### Render default Cursor component

Source: https://motion.dev/docs/cursor

Render the Cursor component to display a default custom cursor on the page. When rendered, it automatically hides the browser's default cursor and replaces it with the Motion cursor.

```jsx
<Cursor />
```

--------------------------------

### Disable Motion component enter animation

Source: https://motion.dev/docs/react-motion-component

Set initial={false} to disable the enter animation and render the component with values from the animate prop. This is useful for server-side rendering or when you want to skip the initial animation.

```javascript
<motion.div initial={false} animate={{ opacity: 0 }} />
```

--------------------------------

### Animate Specific Layout Properties in Motion.dev

Source: https://motion.dev/docs/vue-motion-component

Allows animating only specific layout properties, such as position or size. By setting `layout` to "position" or "size", you can fine-tune which aspects of the component's layout are animated.

```html
<motion.img layout="position" />
```

--------------------------------

### Shared Layout Animation with layoutId

Source: https://motion.dev/docs/vue-layout-animations

Uses the `layoutId` prop to match and animate between two different elements. When a new component with matching `layoutId` is added, it automatically animates from the old component's position, enabling advanced layout transitions.

```vue
<motion.li layoutId="item" />
```

--------------------------------

### Per-Value Overrides with Named Transitions

Source: https://motion.dev/docs/animate

Override global animation options for specific properties by providing named transition objects within the options parameter.

```APIDOC
## FUNCTION `animate` - Named Transitions

### Description
Animation options can be overridden on a per-value basis by providing named transition objects within the main options object. This allows for fine-grained control over individual property animations.

### Function Signature
`animate(element, keyframes, options)`

### Parameters
#### Options Object Properties
- **[propertyName]** (object) - Optional - An object containing specific options (e.g., `duration`, `ease`) for the corresponding `propertyName`.

### Example Usage
```javascript
animate(
  element,
  { x: 100, rotate: 0 },
  {
    duration: 1,
    rotate: { duration: 0.5, ease: "easeOut" }
  }
)
```

### Effect/Output
The `x` property will animate over `1` second with default easing. The `rotate` property will animate over `0.5` seconds with an `"easeOut"` easing function, overriding the global `duration`.
```
// 'x' animates for 1s.
// 'rotate' animates for 0.5s with easeOut.
```
```

--------------------------------

### layoutScroll - Enable Scroll Offset Measurement

Source: https://motion.dev/docs/react-motion-component

Marks scrollable ancestor elements for scroll offset measurement, enabling correct layout animations within scrollable containers. Required for layout animations to function properly in overflow elements.

```jsx
<motion.div layoutScroll style={{ overflow: "scroll" }}>
  <motion.div layout />
</motion.div>
```

--------------------------------

### dragSnapToOrigin

Source: https://motion.dev/docs/react-motion-component

Controls whether the draggable element animates back to its center/origin when released.

```APIDOC
## dragSnapToOrigin

### Description
If `true`, the draggable element will animate back to its center/origin when released.

### Type
`boolean`

### Default
`false`

### Usage Example
```jsx
<motion.div drag dragSnapToOrigin />
```
```

--------------------------------

### dragElastic

Source: https://motion.dev/docs/react-motion-component

Defines the degree of movement allowed outside constraints. Can be a number from 0 to 1, or an object for individual constraint elasticity.

```APIDOC
## dragElastic

### Description
The degree of movement allowed outside constraints. `0` = no movement, `1` = full movement. Can also be set as `false` to disable movement. By passing an object of `top`/`right`/`bottom`/`left`, individual values can be set per constraint. Any missing values will be set to `0`.

### Type
`number` | `boolean` | `object`

### Default
`0.5`

### Parameters
#### Object Parameters
- **left** (number) - Optional - Elasticity for the left constraint.
- **right** (number) - Optional - Elasticity for the right constraint.
- **top** (number) - Optional - Elasticity for the top constraint.
- **bottom** (number) - Optional - Elasticity for the bottom constraint.

### Usage Example
```jsx
<motion.div
  drag
  dragConstraints={{ left: 0, right: 300 }}
  dragElastic={0.2}
/>
```
```

--------------------------------

### Apply Style with Motion Values in Vue

Source: https://motion.dev/docs/vue-motion-component

Use the style prop with motion values and independent transforms for smooth animations. Supports motion values created with useMotionValue() and transform properties like rotate and originX. Enables frame-by-frame animation updates.

```vue
<script setup>
  const x = useMotionValue(30)
</script>

<template>
  <motion.div :style="{ x, rotate: 90, originX: 0.5 }" />
</template>
```

--------------------------------

### Generate random values using `mix` and `Math.random()` in JavaScript

Source: https://motion.dev/docs/mix

The `mix` function can be used in conjunction with `Math.random()` to generate random values within a specified range. Easing functions can further modify the distribution of these random values, allowing for non-linear probability distributions (e.g., `easeOut` for mostly higher numbers, `easeIn` for mostly lower numbers).

```javascript
const x = mix(100, 400, Math.random())

// Mostly higher numbers
mix(0, 50, easeOut(Math.random()))

// Mostly lower numbers
mix(0, 50, easeIn(Math.random()))
```

--------------------------------

### Handle Motion Component Update Events

Source: https://motion.dev/docs/vue-motion-component

The onUpdate callback fires every frame when any value on the motion component changes. Receives a single argument containing the latest animated values, enabling real-time tracking of animation progress.

```vue
<motion.article
  :animate="{ opacity: 1 }"
  @update="latest => console.log(latest.opacity)"
/>
```

--------------------------------

### AnimatePresence propagate Prop

Source: https://motion.dev/docs/react-animate-presence

If set to `true`, exit animations on children will also trigger when this `AnimatePresence` exits from a parent `AnimatePresence`.

```APIDOC
## propagate

### Description
If set to `true`, exit animations on children will also trigger when this `AnimatePresence` exits from a parent `AnimatePresence`. Defaults to `false`.

### Method
Component Prop

### Endpoint
AnimatePresence

### Parameters
#### Request Body
- **propagate** (boolean) - Optional - If `true`, enables nested `AnimatePresence` components to trigger their children's exit animations when the parent `AnimatePresence` unmounts.

### Request Example
```jsx
<AnimatePresence>
  {show ? (
    <motion.section exit={{ opacity: 0 }}>
      <AnimatePresence propagate>
        {/* This exit prop will now fire when show is false */}
        <motion.div exit={{ x: -100 }} />
      </AnimatePresence>
    </motion.section>
  ) : null}
</AnimatePresence>
```

### Response
#### Success Response (N/A)
- This prop controls component behavior, not a direct API response.

#### Response Example
N/A
```

--------------------------------

### Animate `boxShadow` Directly (Less Performant) in JavaScript

Source: https://motion.dev/docs/performance

This JavaScript snippet illustrates animating the `boxShadow` property directly. While functional, animating `boxShadow` can be less performant as it often requires expensive paint operations, potentially leading to janky animations, especially on lower-powered devices.

```javascript
// ❌
animate(element, { boxShadow: "10px 10px black" })
```

--------------------------------

### Animate Full Transform String with WAAPI

Source: https://motion.dev/docs/improvements-to-the-web-animations-api-dx

Demonstrates WAAPI's requirement to animate the full transform string since CSS doesn't offer individual styles for x, scaleX, etc. This prevents separate animations or different animation options for individual transforms.

```javascript
element.animate({ transform: "translateX(50px) scaleX(2)" })
```

--------------------------------

### Transform Motion Values with useTransform Hook

Source: https://motion.dev/docs/vue-motion-value

Create derived motion values by transforming one or more source motion values using useTransform. Maps input ranges to output ranges, enabling synchronized visual property changes like opacity based on drag position without triggering Vue re-renders.

```vue
<script setup>
import { useMotionValue, useTransform} from "motion-v"

const x = useMotionValue(0)
const opacity = useTransform(
x,
[-200, 0, 200],
[0, 1, 0]
)
</script>

<template>
<!-- // Will change opacity as element is dragged left/right -->
<motion.div drag="x" :style="{ x, opacity }" />
</template>
```

--------------------------------

### animate() - Value Animation with Callbacks

Source: https://motion.dev/docs/animate

Animate numeric and color values directly, outputting the latest values to an onUpdate callback. Useful for animating values that don't correspond to DOM properties.

```APIDOC
## animate() - Value Animation

### Description
Animate numeric and color values with callback functions to capture intermediate values. Available in the hybrid version.

### Syntax
```javascript
animate(fromValue, toValue, { onUpdate: callback, ...options })
```

### Parameters
- **fromValue** (number | string) - Required - Starting value (number or color)
- **toValue** (number | string) - Required - Ending value (number or color)
- **options** (object) - Optional - Animation configuration
  - **onUpdate** (function) - Callback receiving latest animated value
  - **duration** (number) - Animation duration in seconds
  - Other standard animate options

### Request Examples

#### Animate Numbers
```javascript
animate(0, 100, {
  onUpdate: latest => console.log(latest)
})
```

#### Animate Colors
```javascript
animate("#fff", "#000", {
  duration: 2,
  onUpdate: latest => console.log(latest)
})
```

### Response
The onUpdate callback receives the current animated value at each frame.
```

--------------------------------

### Handle Pan Gesture Events

Source: https://motion.dev/docs/vue-motion-component

The onPan callback fires when a pan gesture is recognized on the element. Receives PointerEvent and info object containing point, delta, offset, and velocity data. Requires touch-action CSS rule to disable touch scrolling for proper touch input handling.

```vue
function onPan(event, info) {
  console.log(info.point.x, info.point.y)
}

<motion.div @pan="onPan" />
```

--------------------------------

### custom - Pass Data to Dynamic Variants

Source: https://motion.dev/docs/react-motion-component

Passes custom data to variant functions, enabling parameterized animations. Useful for staggered animations where each element receives unique values like delay multipliers.

```jsx
const variants = {
  visible: (custom) => ({
    opacity: 1,
    transition: { delay: custom * 0.2 }
  })
}

return (
  <motion.ul animate="visible">
    <motion.li custom={0} variants={variants} />
    <motion.li custom={1} variants={variants} />
    <motion.li custom={2} variants={variants} />
  </motion.ul>
)
```

--------------------------------

### Animate Motion Values - JavaScript

Source: https://motion.dev/docs/animate

Shows how to animate React motion values. When a motion value is passed to animate(), it is automatically updated with the latest animation values.

```javascript
const x = motionValue(0)

animate(x, 200, { duration: 0.5 })
```

--------------------------------

### Handle Animation Updates with `onUpdate` Callback in Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `onUpdate` callback is triggered on every frame when any value on the `motion` component updates. It provides the latest animated values as an argument, useful for real-time monitoring or side effects.

```javascript
<motion.article
  animate={{ opacity: 1 }}
  onUpdate={latest => console.log(latest.opacity)}
/>
```

--------------------------------

### Apply Drag Animations with whileDrag

Source: https://motion.dev/docs/vue-motion-component

Define animation targets or variant labels to apply while dragging a component. Can be used as a direct animation target object or reference a named variant. Automatically reverts when drag ends.

```vue
<!-- As target -->
<motion.div drag :whileDrag="{ scale: 0.9 }" />

<!-- As variants -->
<motion.div drag whileDrag="dragging" />
```

--------------------------------

### Control Stagger Direction with scrambleText

Source: https://motion.dev/docs/scramble-text

Illustrates using the `from` option within `stagger()` to specify the direction from which characters are revealed during a `scrambleText` animation. This allows for effects like revealing text from the 'center' outwards.

```javascript
scrambleText(element, {
  delay: stagger(0.05, { from: "center" }),
  duration: 0.5
})
```

--------------------------------

### Animate Transform Properties - JavaScript

Source: https://motion.dev/docs/animate

Shows how to animate independent transform axes using the hybrid version of animate(). Supports translate (x, y, z), scale, rotate, skew, and perspective transformations.

```javascript
animate("div", { rotate: 360 })
```

--------------------------------

### Enable dragSnapToOrigin animation

Source: https://motion.dev/docs/react-motion-component

When set to true, the draggable element animates back to its center or origin position when the drag gesture is released. Default value is false.

```JSX
<motion.div drag dragSnapToOrigin />
```

--------------------------------

### Configure dragElastic movement outside constraints

Source: https://motion.dev/docs/react-motion-component

Controls the degree of movement allowed outside drag constraints. Values range from 0 (no movement) to 1 (full movement), with default 0.5. Can be set as false to disable or as an object with individual top/right/bottom/left values.

```JSX
<motion.div
  drag
  dragConstraints={{ left: 0, right: 300 }}
  dragElastic={0.2}
/>
```

--------------------------------

### Jump to value immediately without animation

Source: https://motion.dev/docs/react-use-spring

Use the .jump() method to update the motion value immediately to a new target without triggering the spring animation. Useful for instant position changes or initialization.

```javascript
x.jump(50)
y.jump("0vh")
```

--------------------------------

### Handle Hover End Events

Source: https://motion.dev/docs/vue-motion-component

The onHoverEnd callback fires when a pointer stops hovering over the component. Receives the triggering PointerEvent as an argument.

```vue
<motion.div @hoverEnd="(event) => console.log(event)" />
```

--------------------------------

### Configure Automatic Reduced Motion in React with MotionConfig

Source: https://motion.dev/docs/react-accessibility

Demonstrates how to automatically adjust animations based on user preferences by setting the `reducedMotion` prop to "user" on the `MotionConfig` component. This disables transform and layout animations while preserving opacity and background color animations across all child `motion` components.

```javascript
import { MotionConfig } from "framer-motion"

export function App({ children }) {
  return (
    <MotionConfig reducedMotion="user">
      {children}
    </MotionConfig>
  )
}
```

--------------------------------

### Typewriter Dynamic Content Backspace All in React

Source: https://motion.dev/docs/react-typewriter

Configures the `Typewriter` component to immediately remove all mismatching content when its `children` prop changes. This option is useful for quick transitions between dynamic text values.

```jsx
<Typewriter backspace="all">{text}</Typewriter>
```

--------------------------------

### Disable Initial Animations with AnimatePresence `initial` Prop (React)

Source: https://motion.dev/docs/react-animate-presence

The `initial={false}` prop on AnimatePresence prevents any initial animations from running on children that are present when the component first renders. This is useful for controlling when animations should occur, typically only for mount/unmount transitions.

```jsx
<AnimatePresence initial={false}>
  <Slide key={activeItem.id} />
</AnimatePresence>
```

--------------------------------

### Apply spring animation to DOM element via style attribute

Source: https://motion.dev/docs/css

Set spring transitions on DOM elements at runtime by modifying the element's style property before changing other CSS values. Useful for dynamic animations triggered by user interactions.

```javascript
const element = document.querySelector("button")

element.style.transition = "transform " + spring(0.3)
element.style.transform = "scale(1.2)"
```

--------------------------------

### Custom Motion component with ref prop (React 19)

Source: https://motion.dev/docs/react-motion-component

In React 19, pass ref directly via props to the element you want to animate. This simplified approach eliminates the need for forwardRef wrapper.

```javascript
const Component = (props) => {
  return <div ref={props.ref} />
}
```

--------------------------------

### Layout Animation in Scrollable Elements

Source: https://motion.dev/docs/vue-layout-animations

Uses the `layoutScroll` prop on a scrollable container to correctly measure and animate child elements. This accounts for the element's scroll offset when calculating layout changes.

```vue
<motion.div layoutScroll :style="{ overflow: 'scroll' }" />
```

--------------------------------

### Check Motion Value Animation Status with isAnimating

Source: https://motion.dev/docs/vue-motion-value

Determine if a motion value is currently animating using the isAnimating method. Returns true if an active animation is running, false otherwise.

```javascript
x.isAnimating()
```

--------------------------------

### Set Delay Between Animation Repeats in Framer Motion

Source: https://motion.dev/docs/vue-transitions

Specifies the duration, in seconds, to wait between each repetition of an animation. This property is active when `repeat` is set to a value greater than 0. Default is 0.

```Framer Motion
<motion.div
  :animate="{ rotate: 180 }"
  :transition="{ repeat: Infinity, repeatDelay: 1 }"
/>
```

--------------------------------

### dragConstraints

Source: https://motion.dev/docs/react-motion-component

Applies constraints on the draggable area. Can be an object of pixel values or a ref to another element's bounding box.

```APIDOC
## dragConstraints

### Description
Applies constraints on the draggable area. Set as an object of optional `top`, `left`, `right`, and `bottom` values, measured in pixels, or as a `ref` to another element to use its bounding box as the draggable constraints.

### Type
`object` | `React.RefObject`

### Parameters
#### Object Parameters
- **left** (number) - Optional - Left constraint in pixels.
- **right** (number) - Optional - Right constraint in pixels.
- **top** (number) - Optional - Top constraint in pixels.
- **bottom** (number) - Optional - Bottom constraint in pixels.

#### Ref Parameter
- **ref** (React.RefObject) - Optional - A ref to another DOM element whose bounding box will be used as constraints.

### Usage Example
```jsx
<motion.div
  drag="x"
  dragConstraints={{ left: 0, right: 300 }}
/>

const MyComponent = () => {
  const constraintsRef = useRef(null)

  return (
     <motion.div ref={constraintsRef}>
         <motion.div drag dragConstraints={constraintsRef} />
     </motion.div>
  )
}
```
```

--------------------------------

### Set Default Transition for Motion Component

Source: https://motion.dev/docs/vue-motion-component

Configure the default transition type and settings for a motion component. This transition is used for all animation props (animate, whileHover, etc.) that don't have their own transition defined.

```vue
<motion.div :transition="{ type: 'spring' }" :animate="{ scale: 1.2 }" />
```

--------------------------------

### AnimateActivity with Tab Component

Source: https://motion.dev/docs/react-animate-activity

Shows how to use AnimateActivity with a reusable Tab component that includes entry and exit animations. The parent component controls visibility while the child component defines animation behavior.

```jsx
<AnimateActivity mode={isVisible ? "visible" : "hidden"}>
  <Tab />
</AnimateActivity>

function Tab() {
  return (
    <motion.div
      initial={{ opacity: 0 }}
      animate={{ opacity: 1 }}
      exit={{ opacity: 0 }}
    />
  )
}
```

--------------------------------

### Create collapsible accordion item with Motion Vue layout

Source: https://motion.dev/docs/vue-layout-group

Demonstrates a single accordion item component that uses the motion.div with layout prop to animate layout changes on click. The component manages its own open/closed state and re-renders content conditionally, triggering automatic layout animations.

```vue
<script setup>
const isOpen = ref(false)
</script>
<template>
<motion.div
layout
@click="isOpen=!isOpen"
>
<motion.h2 layout>{{header}}</motion.h2>
{{isOpen ? content : null}}
</motion.div>
</template>
```

--------------------------------

### Playing and Resuming Animations (JavaScript)

Source: https://motion.dev/docs/animate

The `play()` method resumes a paused animation from its current `time` or restarts a finished animation from the beginning. This provides control over the animation's active state.

```javascript
animation.pause()

// Will resume from 1 second
animation.time = 1
animation.play()

// Will play from start
await animation
animation.play()
```

--------------------------------

### Adjust keyframe positioning with `times` option in Motion.dev

Source: https://motion.dev/docs/animate

Demonstrates using the `times` option to precisely control the timing of each keyframe within an animation. Values in the `times` array (0-1) map to the animation's progress, allowing uneven keyframe distribution.

```javascript
animate(
  element,
  { x: [0, 100, 0] },
  { times: [0, 0.3, 1] }
)
```

--------------------------------

### Animation State Persistence

Source: https://motion.dev/docs/improvements-to-the-web-animations-api-dx

Motion automatically persists animation state to the target value after completion, avoiding WAAPI's unintuitive behavior where animations revert to initial state. This eliminates the need for manual Promise handlers or style manipulation.

```JavaScript
import { animate } from "motion/dom"

// WAAPI reverts to initial state without fill: "forwards"
element.animate({ opacity: 0 })

// Motion automatically persists to target state
animate(element, { opacity: 0 })
```

--------------------------------

### Fixing Exit Animations: Avoid Conditional `AnimatePresence` Root in Vue

Source: https://motion.dev/docs/vue-animate-presence

This snippet illustrates an incorrect pattern where `AnimatePresence` itself is conditionally rendered using `v-if`. When `AnimatePresence` unmounts, it cannot control exit animations for its children, leading to broken animation behavior.

```html
<AnimatePresence v-if="isVisible">
  <Component />
</AnimatePresence>
```

--------------------------------

### Default Value Types Handling

Source: https://motion.dev/docs/improvements-to-the-web-animations-api-dx

Motion automatically handles default unit types for animatable values, eliminating the need to manually specify units like 'px' for common properties. This differs from WAAPI which requires explicit unit types.

```JavaScript
import { animate } from "motion/dom"

// WAAPI requires explicit units
element.animate({ width: "100px" })
element.animate({ width: 100 }) // Error!

// Motion handles default types automatically
animate(element, { width: 100 })
```

--------------------------------

### animate() - SVG Path Animations (Hybrid)

Source: https://motion.dev/docs/animate

Perform line drawing animations on SVG elements using special path properties. Supports pathLength, pathSpacing, and pathOffset for creating stroke animation effects.

```APIDOC
## animate() - SVG Path Animations

### Description
Create line drawing animations on SVG elements using path-specific animation properties. Available only in the hybrid version.

### Supported SVG Elements
- circle
- ellipse
- line
- path
- polygon
- polyline
- rect

### Path Animation Properties
- **pathLength** (number) - Progress value between 0 and 1 representing total path length
- **pathSpacing** (number) - Spacing along the path as progress value (0-1)
- **pathOffset** (number) - Offset along the path as progress value (0-1)

### Request Example
```javascript
animate("circle", { pathLength: [0, 1] })
animate("path", { pathLength: [0, 1], pathOffset: [0, 1] })
animate("rect", { pathLength: 1 }, { duration: 2 })
```

### Notes
All path animation values are set as progress values between 0 and 1, where 1 represents the total length of the path.
```

--------------------------------

### Configure Spring Rest Delta Parameter

Source: https://motion.dev/docs/animate

Sets the distance threshold for animation completion with a default value of 0.01. Animation ends when distance falls below this value and speed is below restSpeed. This ensures animations complete when they reach their target within acceptable tolerances.

```javascript
animate(
  ".my-element",
  { x: 200 },
  { type: "spring", restDelta: 0.5 }
)
```

--------------------------------

### Handle onDragEnd callback

Source: https://motion.dev/docs/react-motion-component

Callback function that fires when a drag gesture ends. Receives the triggering PointerEvent and info object containing delta, offset, point, and velocity properties.

```JSX
<motion.div drag onDragEnd={(event, info) => console.log(info.delta.x)} />
```

--------------------------------

### Fixing Exit Animations: Use Unique ID as `key` in Vue `v-for` with `AnimatePresence`

Source: https://motion.dev/docs/vue-animate-presence

This snippet shows the correct way to assign a unique `key` to components within a `v-for` loop inside `AnimatePresence`. By using a stable identifier like `item.id`, exit animations will function correctly even if the list items reorder.

```html
<AnimatePresence>
  <Componen v-for="(item,index) in items" :key="item.id" />
</AnimatePresence>
```

--------------------------------

### Animate Layout Transitions with `layoutId` in Motion.dev

Source: https://motion.dev/docs/vue-motion-component

Enables shared layout animations between `motion` components. When a new element with a matching `layoutId` enters the DOM, it animates from the previous element's state, facilitating smooth transitions and crossfades.

```html
 <motion.li v-for="item in items" layout>
    {{item.name}}
    <motion.div v-if="item.isSelected" layoutId="underline" />
 </motion.li>
```

--------------------------------

### Implement BezierCurveEditor as Controlled Component (React)

Source: https://motion.dev/docs/studio-sdk-bezier-curve-editor

This snippet showcases how to use `BezierCurveEditor` as a controlled component in React by integrating it with the `useState` hook. It initializes the bezier curve state and passes the state variable to the `curve` prop, while the state updater function is provided to the `onChange` prop.

```jsx
const [curve, setCurve] = useState([0.3, 0, 0.6, 1])

return <BezierCurveEditor curve={curve} onChange={setCurve} />
```

--------------------------------

### Animate SVG Paths - JavaScript

Source: https://motion.dev/docs/animate

Shows line drawing animations for SVG elements using pathLength, pathSpacing, and pathOffset properties. Values are set as progress between 0 and 1, compatible with circle, ellipse, line, path, polygon, polyline, and rect elements.

```javascript
animate("circle", { pathLength: [0, 1] })
```

--------------------------------

### Update useSpring value with set() method

Source: https://motion.dev/docs/react-use-spring

Update the spring motion value using the .set() method, which will animate the value to the new target with the defined spring animation. The animation follows spring physics rather than linear interpolation.

```javascript
x.set(100)
y.set("50vh")
```

--------------------------------

### Animate CSS Variables - JavaScript

Source: https://motion.dev/docs/animate

Demonstrates animating CSS variables using the hybrid version of animate(). The hybrid version supports all browsers, while the mini version only works with registered CSS properties in modern browsers.

```javascript
animate(element, { "--rotate": "360deg" })
```

--------------------------------

### Handle Tap Cancel Event with `onTapCancel` Callback in Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `onTapCancel` callback function is invoked when a pointer stops pressing the component but was released outside the component's bounds. It provides the triggering `PointerEvent` object, useful for handling cancelled tap gestures.

```javascript
<motion.div onTapCancel={(event) => console.log(event)} />
```

--------------------------------

### Handle Element Leaving Viewport in Motion.dev

Source: https://motion.dev/docs/vue-motion-component

Defines a callback function that executes when a `motion` component leaves the viewport. It receives an `IntersectionObserverEntry` object, providing detailed information about the intersection event for custom logic.

```html
<motion.div @viewportLeave="(entry) => console.log(entry.intersectionRect)" />
```

--------------------------------

### Control ScrambleText Stagger Direction in React

Source: https://motion.dev/docs/react-scramble-text

Shows how to customize the direction of the staggered animation using the `from` option within Motion's `stagger` function. This allows characters to animate from specific points like the 'center'.

```jsx
<ScrambleText
  delay={stagger(0.05, { from: "center" })}
  duration={0.5}
>
  Hello world!
</ScrambleText>
```

--------------------------------

### Compose multiple derived motionValues for complex transformations in JavaScript

Source: https://motion.dev/docs/transform-value

This snippet demonstrates the composition capabilities of `transformValue`. It shows how a `motionValue` derived from two others (`rotate`) can itself be used as an input to another `transformValue` (`transform`), enabling the creation of complex, interdependent animations.

```javascript
const x = motionValue(0)
const y = motionValue(0)
const rotate = transformValue(() => x.get() + y.get())
const transform = transformValue(() => `translate3d(${x.get()}px ${y.get()}px 0) rotate(${rotate.get()}deg)`)
```

--------------------------------

### layoutId - Shared Element Animation

Source: https://motion.dev/docs/react-motion-component

Enables layout animations and creates shared element transitions. When a new element with matching layoutId enters the DOM, it animates from the previous element's position and size. Remaining elements crossfade.

```jsx
{items.map(item => (
   <motion.li layout>
      {item.name}
      {item.isSelected && <motion.div layoutId="underline" />}
   </motion.li>
))}
```

--------------------------------

### animate() - CSS Variables Animation (Hybrid)

Source: https://motion.dev/docs/animate

Animate CSS custom properties (variables) across all browsers. The hybrid version supports all CSS variables, while the mini version only supports registered CSS properties in modern browsers.

```APIDOC
## animate() - CSS Variables

### Description
Animate CSS custom properties (variables) with full browser compatibility in the hybrid version.

### Syntax
```javascript
animate(element, { "--variable-name": value }, options?)
```

### Parameters
- **element** (Element | string) - Required - Target element or CSS selector
- **properties** (object) - Required - CSS variables as key-value pairs (prefix with --)
- **options** (object) - Optional - Animation configuration

### Request Example

#### Hybrid Version (All Browsers)
```javascript
animate(element, { "--rotate": "360deg" })
animate(".container", { "--color": "#ff0000", "--opacity": "0.5" })
```

#### Mini Version (Registered Properties Only)
Mini version can only animate registered CSS properties in modern browsers.

### Browser Support
- **Hybrid**: All browsers
- **Mini**: Modern browsers with registered CSS properties support
```

--------------------------------

### Integrating Ticker with Scroll Position in Vue

Source: https://motion.dev/docs/vue-ticker

This Vue snippet illustrates how to create a scroll-driven Ticker animation. It utilizes the `useScroll()` composable to obtain the current `scrollY` value and binds it to the Ticker's `offset` prop, enabling the ticker's movement to be controlled by the page's scroll position.

```vue
<script setup>
const { scrollY } = useScroll()
</script>

<template>
 <Ticker :offset="scrollY" />  
</template>
```

--------------------------------

### Animate JavaScript Objects - JavaScript

Source: https://motion.dev/docs/animate

Demonstrates animating plain JavaScript objects and complex objects like Three.js Object3D instances. Any object with numeric or color properties can be animated.

```javascript
const values = {
  x: 100,
  color: "#f00"
}

animate(values, { x: 200, color: "#00f" })

// Three.js example
const camera = new THREE.Camera()

animate(camera.rotation, { y: 360 }, { duration: 10 })
```

--------------------------------

### Custom Motion component with forwardRef (React 18)

Source: https://motion.dev/docs/react-motion-component

Wrap a React component with forwardRef and pass the ref to the element you want to animate. This enables motion animation capabilities on custom components in React 18.

```javascript
const Component = React.forwardRef((props, ref) => {
  return <div ref={ref} />
})
```

--------------------------------

### Apply Styles with Motion Values in React Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `style` prop in Framer Motion extends React DOM's `style` prop, allowing direct use of motion values and independent transforms. This enables dynamic styling based on animation states or user interactions.

```javascript
const x = useMotionValue(30)

return <motion.div style={{ x, rotate: 90, originX: 0.5 }} />
```

--------------------------------

### onDragEnd

Source: https://motion.dev/docs/react-motion-component

Callback function that fires when a drag gesture ends.

```APIDOC
## onDragEnd

### Description
Callback function that fires when a drag gesture ends. Provided the triggering `PointerEvent` and `info` object.

### Type
`(event: PointerEvent, info: PanInfo) => void`

### Parameters
- **event** (PointerEvent) - The original DOM `PointerEvent` that triggered the drag end.
- **info** (PanInfo) - An object containing drag-related information at the end of the drag.

### Usage Example
```jsx
<motion.div drag onDragEnd={(event, info) => console.log(info.delta.x)} />
```
```

--------------------------------

### Define Animation Variants in Motion Component

Source: https://motion.dev/docs/vue-motion-component

Create named animation states using the variants property. Each variant defines animation properties and transitions that can be triggered via the animate prop. Supports conditional animation switching based on component state.

```vue
<script setup>
  const variants = {
    active: {
        backgroundColor: "#f00"
    },
    inactive: {
      backgroundColor: "#fff",
      transition: { duration: 2 }
    }
  }
</script>

<template>
  <motion.div
    :variants="variants"
    :animate="isActive ? 'active' : 'inactive'"
  />
</template>
```

--------------------------------

### Set `tween` animation type with Motion.dev Hybrid `animate`

Source: https://motion.dev/docs/animate

Demonstrates setting the `type` option to `"tween"` for the Hybrid `animate` function. This configures a duration-based animation with a specified duration, suitable for linear or eased transitions.

```javascript
animate("path", { pathLength: 1 }, { duration: 2, type: "tween" })
```

--------------------------------

### Detect Animation Completion with `onAnimationComplete` Callback in Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `onAnimationComplete` callback fires when any animation (excluding layout animations) finishes. It receives the target or variant name of the completed animation, enabling post-animation actions.

```javascript
<motion.circle
  animate={{ r: 10 }}
  onAnimationComplete={latest => console.log(latest.r)}
/>
```

--------------------------------

### Group accordion items with LayoutGroup for coordinated animations

Source: https://motion.dev/docs/react-layout-group

Wraps multiple accordion items in a LayoutGroup component to enable coordinated layout animations. When one item's state changes, siblings are aware of layout changes and animate accordingly.

```jsx
import { LayoutGroup } from "motion/react"

function Accordion() {
  return (
    <LayoutGroup>
      <ToggleContent />
      <ToggleContent />
    </LayoutGroup>
  )
}
```

--------------------------------

### Adjust Mass for Spring Animation in Framer Motion

Source: https://motion.dev/docs/vue-transitions

Defines the mass of the moving object in a spring animation. Higher mass values result in a more lethargic and slower movement. Default is 1.

```Framer Motion
<motion.feTurbulence
  :animate="{ baseFrequency: 0.5 }"
  :transition="{ type: 'spring', mass: 0.5 }"
/>
```

--------------------------------

### onDrag

Source: https://motion.dev/docs/react-motion-component

Callback function that fires when the drag gesture is recognized and the element is being dragged.

```APIDOC
## onDrag

### Description
Callback function that fires when the drag gesture is recognised on this element.

### Type
`(event: PointerEvent, info: PanInfo) => void`

### Parameters
- **event** (PointerEvent) - The original DOM `PointerEvent` that triggered the drag.
- **info** (PanInfo) - An object containing drag-related information.

### Usage Example
```jsx
function onDrag(event, info) {
  console.log(info.point.x, info.point.y)
}

<motion.div drag onDrag={onDrag} />
```

### Notes
`info` object contains `x` and `y` point values for the following:
- **point**: Relative to the device or page.
- **delta**: Distance since the last event.
- **offset**: Distance from the original event.
- **velocity**: Current velocity of the pointer.
```

--------------------------------

### Configure hover with passive option

Source: https://motion.dev/docs/hover

Set the passive option to false to enable event.preventDefault() calls, though this reduces gesture performance. Default is true.

```javascript
hover(element, callback, { passive: false })
```

--------------------------------

### Use MotionValue for performance optimization

Source: https://motion.dev/docs/react-motion-component

Use useMotionValue hook to create motion values that animate without triggering React re-renders. This approach is more performant than using React state for frequently updated style values. Motion values can be updated with the .set() method without causing component re-renders.

```javascript
const x = useMotionValue(0)

useEffect(() => {
  // Won't trigger a re-render!
  const timeout = setTimeout(() => x.set(100), 1000)

  return () => clearTimeout(timeout)
}, [])

return <motion.div style={{ x }} />
```

--------------------------------

### Sequence Exit Animations with Variants

Source: https://motion.dev/docs/react-animate-activity

Demonstrates sequencing exit animations through a component tree using variants and the stagger function. Child list items animate out in sequence when AnimateActivity mode changes to 'hidden'.

```jsx
<AnimateActivity mode={isVisible ? "visible" : "hidden"}>
  <motion.ul
    exit="hidden"
    variants={{
      hidden: { delayChildren: stagger(0.1) }
    }}
  >
    {items.map(item => (
      <motion.li
        variants={{ hidden: { opacity: 0 }}}
      >
        {item.title}
      </motion.li>
    ))}
  </motion.ul>
</AnimateActivity>
```

--------------------------------

### Set Rest Speed for Spring Animation Termination in Framer Motion

Source: https://motion.dev/docs/vue-transitions

Determines the absolute speed threshold (in units per second) below which the animation will end. The animation also requires the delta to be smaller than `restDelta` for termination. Default is 0.1.

```Framer Motion
<motion.div
  :animate="{ rotate: 180 }"
  :transition="{ type: 'spring', restSpeed: 0.5 }"
/>
```

--------------------------------

### Advanced Typewriter Configuration in Vue

Source: https://motion.dev/docs/vue-typewriter

Typewriter component with customized animation parameters including typing speed, variance for natural pauses, backspace behavior, and cursor blink speed. All animation and typing behaviors can be independently modified.

```vue
<Typewriter
  speed="fast"
  :variance="0.8"
  backspace="word"
  :cursorBlinkSpeed="2"
>
  {{text}}
</Typewriter>
```

--------------------------------

### AnimatePresence `popLayout` Mode for Reflowing Elements (React)

Source: https://motion.dev/docs/react-animate-presence

The `popLayout` mode in AnimatePresence causes exiting elements to be 'popped' out of the document flow, allowing surrounding elements to reflow immediately. This mode pairs effectively with the `layout` prop for smooth transitions of remaining elements. When using custom components as immediate children, they must be wrapped in `React.forwardRef`.

```jsx
<AnimatePresence>
  {items.map(item => (
    <motion.li layout exit={{ opacity: 0 }} />
  ))}
</AnimatePresence>
```

--------------------------------

### Style EasingCurve path with color and width

Source: https://motion.dev/docs/studio-sdk-easing-curve

Customize the appearance of the drawn curve line using the color prop for the line color and pathWidth prop for the line thickness in pixels.

```javascript
<EasingCurve curve={curve} color="#fff" pathWidth={2} />
```

--------------------------------

### dragListener

Source: https://motion.dev/docs/react-motion-component

Determines whether to trigger the drag gesture from event listeners on the draggable element itself.

```APIDOC
## dragListener

### Description
Determines whether to trigger the drag gesture from event listeners. If passing `dragControls`, setting this to `false` will ensure dragging can only be initiated by the controls, rather than a `pointerdown` event on the draggable element.

### Type
`boolean`

### Default
`true` (implicitly, if `dragControls` is not used)
```

--------------------------------

### Detect Animation Complete Events

Source: https://motion.dev/docs/vue-motion-component

The onAnimationComplete callback triggers when any animation finishes (excluding layout animations). Receives the target or variant name of the completed animation as an argument.

```vue
<motion.circle
  :animate="{ r: 10 }"
  @animationComplete="latest => console.log(latest.r)"
/>
```

--------------------------------

### Stopping inView Viewport Detection (JavaScript)

Source: https://motion.dev/docs/inview

Explains that `inView` returns a function which, when invoked, will stop all further viewport detection for the associated elements. This is crucial for performance optimization and resource management when detection is no longer needed.

```javascript
const stop = inView(element, callback)

stop()
```

--------------------------------

### animate() - Transform Animations (Hybrid)

Source: https://motion.dev/docs/animate

The hybrid version of animate() can animate every transform axis independently, including translate, scale, rotate, skew, and perspective properties.

```APIDOC
## animate() - Transform Animations

### Description
Animate independent transform properties with precise control over each axis. Available only in the hybrid version (18kb).

### Supported Transform Properties

#### Translate
- **x** (number) - Horizontal translation in pixels
- **y** (number) - Vertical translation in pixels
- **z** (number) - Depth translation in pixels

#### Scale
- **scale** (number) - Uniform scale on all axes
- **scaleX** (number) - Horizontal scale
- **scaleY** (number) - Vertical scale

#### Rotate
- **rotate** (number) - 2D rotation in degrees
- **rotateX** (number) - 3D rotation around X axis
- **rotateY** (number) - 3D rotation around Y axis
- **rotateZ** (number) - 3D rotation around Z axis

#### Skew
- **skewX** (number) - Horizontal skew in degrees
- **skewY** (number) - Vertical skew in degrees

#### Perspective
- **transformPerspective** (number) - Perspective distance in pixels

### Request Example
```javascript
animate("div", { rotate: 360 })
animate(element, { x: 100, y: 50, rotate: 45 })
animate("box", { scaleX: 1.5, rotateZ: 180 }, { duration: 1 })
```
```

--------------------------------

### inherit - Control Variant Propagation

Source: https://motion.dev/docs/react-motion-component

When set to false, prevents a component from inheriting or propagating parent variant changes. Useful for isolating component animations from parent animation contexts.

```jsx
<motion.div inherit={false} />
```

--------------------------------

### Pass Motion Value to SVG Attributes

Source: https://motion.dev/docs/react-motion-value

Shows how to apply motion values to SVG element attributes directly, rather than through the style prop. Motion values can be used with any SVG attribute like cx, cy, r, etc.

```jsx
<motion.circle cx={cx} />
```

--------------------------------

### transformTemplate - Customize Transform Order

Source: https://motion.dev/docs/react-motion-component

Customizes the order and format of CSS transforms (translate, scale, rotate, skew). Accepts function with transform values or generated string, returning modified transform string.

```jsx
<motion.div
  style={{ x: 0, rotate: 180 }}
  transformTemplate={
    ({ x, rotate }) => `rotate(${rotate}deg) translateX(${x}px)`
  }
/>
```

```jsx
<motion.div
  style={{ x: 0, rotate: 180 }}
  transformTemplate={
    (latest, generated) => `translate(-50%, -50%) ${generated}`
  }
/>
```

--------------------------------

### Group accordion items with LayoutGroup for coordinated animations

Source: https://motion.dev/docs/vue-layout-group

Shows how to wrap multiple accordion items in a LayoutGroup component so they can detect and animate each other's layout changes. Without LayoutGroup, sibling components have no way of knowing when their siblings update state.

```vue
<!-- Accordion -->
<template>
<LayoutGroup>
<ToggleContent />
<ToggleContent />
</LayoutGroup>
</template>
```

--------------------------------

### Handle onDrag callback with pointer and info data

Source: https://motion.dev/docs/vue-motion-component

The onDrag callback fires when a drag gesture is recognized. It receives the PointerEvent and an info object containing point (relative to device/page), delta (distance since last event), offset (distance from original event), and velocity (current pointer velocity).

```vue
function onDrag(event, info) {
  console.log(info.point.x, info.point.y)
}

<motion.div drag @drag="onDrag" />
```

--------------------------------

### Apply single motion value to multiple styles

Source: https://motion.dev/docs/style-effect

A single motion value can be applied to multiple CSS properties on the same or different elements, enabling synchronized style updates across the DOM.

```javascript
const progress = motionValue(0)

styleEffect("#progress", {
  opacity: progress,
  scaleX: progress
})
```

--------------------------------

### Adjusting Animation Playback Speed (JavaScript)

Source: https://motion.dev/docs/animate

The `speed` property controls the playback rate of the animation. A value of `1` is normal speed, `0.5` is half speed, `2` doubles the rate, and `-1` reverses playback. This allows for dynamic speed adjustments.

```javascript
const animation = animate(element, { opacity: 0 })

const currentSpeed = animation.speed

// Double current speed
animation.speed = currentSpeed * 2
```

--------------------------------

### Customize Transform Order with `transformTemplate` in Motion.dev (Generated String)

Source: https://motion.dev/docs/vue-motion-component

Enables modification of the automatically generated CSS transform string. This function receives both the latest transform values and the default generated string, allowing for additional transformations like centering.

```html
<!-- // Or the generated transform string -->
<motion.div
  :style="{ x: 0, rotate: 180 }"
  :transformTemplate="(latest, generated) => `translate(-50%, -50%) ${generated}`"
/>
```

--------------------------------

### Glide Animation with Custom Velocity

Source: https://motion.dev/docs/glide

Shows how to override the default velocity by passing a custom velocity value (in units per second) to the glide() function. This is useful for carousel animations or when you need precise control over the initial momentum.

```javascript
animate(
  "#carousel",
  { x: 100 },
  { easing: glide({ velocity: 1000 }) }
)
```

--------------------------------

### Set Rest Delta for Spring Animation Termination in Framer Motion

Source: https://motion.dev/docs/vue-transitions

Defines the distance threshold below which the animation will end. For termination, the speed must also be below `restSpeed`. When these conditions are met, the spring animation concludes. Default is 0.01.

```Framer Motion
<motion.div
  :animate="{ rotate: 180 }"
  :transition="{ type: 'spring', restDelta: 0.5 }"
/>
```

--------------------------------

### stop() Method

Source: https://motion.dev/docs/animate

Stops the animation and commits all animated values to the element via inline styles. Stopped animations cannot be restarted.

```APIDOC
## stop() Method

### Description
Stops the animation. Any values being animated via the Web Animations API will be committed to the element via `style`. Stopped animations cannot be restarted.

### Method
- **stop()** - Stops animation and commits values to element styles

### Usage Example
```javascript
const animation = animate(element, { opacity: 0 })
animation.stop()
```
```

--------------------------------

### Conditionally Disable Autoplay for Video in React

Source: https://motion.dev/docs/react-accessibility

Demonstrates how to use the `useReducedMotion` hook to control the `autoplay` attribute of an HTML `<video>` element. If reduced motion is enabled, the video will not autoplay, enhancing accessibility for users sensitive to motion.

```javascript
function BackgroundVideo() {
  const shouldReduceMotion = useReducedMotion()

  return <video autoplay={!shouldReduceMotion} />
}
```

--------------------------------

### Configure dragElastic for constraint boundary movement

Source: https://motion.dev/docs/vue-motion-component

Control the degree of movement allowed outside drag constraints using dragElastic (0 = no movement, 1 = full movement). Default is 0.5. Can be set as false to disable movement, or as an object with individual top/right/bottom/left values.

```vue
<motion.div
  drag
  :dragConstraints="{ left: 0, right: 300 }"
  :dragElastic="0.2"
/>
```

--------------------------------

### Handle Press Events Inside Component

Source: https://motion.dev/docs/vue-motion-component

The onPress callback fires when a pointer stops pressing and is released inside the component. Receives the triggering PointerEvent as an argument.

```vue
<motion.div @press="(event) => console.log(event)" />
```

--------------------------------

### Continuous Rotation with `useTransform` and `clamp: false` (React)

Source: https://motion.dev/docs/react-use-transform

Uses `useTransform` with `useScroll` and `clamp: false` to create a continuous rotation effect. For every 100px scrolled, the element rotates another 360 degrees, demonstrating non-clamped range mapping.

```javascript
const { scrollY } = useScroll()
const rotate = useTransform(
  scrollY,
  [0, 100],
  [0, 360],
  { clamp: false }
)
```

--------------------------------

### Apply Drag Animations with `whileDrag` in Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `whileDrag` prop defines an animation state or variant label to apply while the component is being dragged. It can be used to animate properties directly or trigger predefined variants, providing visual feedback during dragging.

```javascript
// As target
<motion.div drag whileDrag={{ scale: 0.9 }} />
```

```javascript
// As variants
<motion.div drag whileDrag="dragging" />
```

--------------------------------

### Applying Layout Correction to Nested Elements in Motion

Source: https://motion.dev/docs/vue-layout-animations

To prevent undesirable stretching of content when animating `width` and `height` with `scale`, apply the `layout` prop to both the parent and child `motion` components. This enables Motion's scale correction mechanism for nested elements like images or text.

```JSX
<motion.section layout>
  <motion.img layout />
</motion.section>
```

--------------------------------

### animate() - Object Animation

Source: https://motion.dev/docs/animate

Animate JavaScript objects and complex structures like Three.js Object3D instances. Any object with numeric or color properties can be animated.

```APIDOC
## animate() - Object Animation

### Description
Animate JavaScript objects and complex structures. Supports any object with numeric or color properties, including Three.js objects.

### Syntax
```javascript
animate(object, targetProperties, options?)
```

### Parameters
- **object** (object) - Required - Object to animate
- **targetProperties** (object) - Required - Target values for object properties
- **options** (object) - Optional - Animation configuration

### Request Examples

#### Simple Object
```javascript
const values = {
  x: 100,
  color: "#f00"
}

animate(values, { x: 200, color: "#00f" })
```

#### Three.js Object
```javascript
const camera = new THREE.Camera()
animate(camera.rotation, { y: 360 }, { duration: 10 })
```

### Notes
Any object can be animated as long as it contains numeric or color properties that can be interpolated.
```

--------------------------------

### Animation Controls Overview

Source: https://motion.dev/docs/animate

The animate() function returns an animation object with playback controls. These controls allow you to manage animation state, timing, speed, and completion through various methods and properties.

```APIDOC
## Animation Controls API

### Description
The `animate()` function returns animation playback controls that can be used to manage animation state and behavior.

### Basic Usage
```javascript
const animation = animate(element, { opacity: 1 })

animation.time = 0.5
animation.stop()
```

### Available Properties and Methods
- `duration` - Read-only duration of a single animation iteration
- `time` - Get/set current animation time
- `speed` - Get/set animation playback speed
- `pause()` - Pause the animation
- `play()` - Resume or restart the animation
- `complete()` - Jump to animation end state
- `cancel()` - Revert to initial state
- `stop()` - Stop animation and commit values
- `then()` - Promise-like API for completion
```

--------------------------------

### AnimateActivity with Pop Layout Mode

Source: https://motion.dev/docs/react-animate-activity

Configures AnimateActivity with layoutMode set to 'pop' to immediately remove the exiting element from the document layout. This allows surrounding elements to reflow while the exit animation completes.

```jsx
<AnimateActivity
  mode={isVisible ? "visible" : "hidden"}
  layoutMode="pop"
/>
```

--------------------------------

### Pass Motion Values to Motion Components

Source: https://motion.dev/docs/vue-motion-value

Apply motion values to motion components via the style prop for DOM elements or directly as attributes for SVG elements. The same motion value can be passed to multiple components to synchronize motion across them.

```vue
<motion.li :style="{ x }" />
```

```vue
<motion.circle :cx="cx" />
```

--------------------------------

### Define a Tween Transition Type in Motion (Vue)

Source: https://motion.dev/docs/vue-transitions

This snippet shows how to explicitly set the `type` property of a transition to `'tween'`. Tween animations are duration-based and use easing curves, making them suitable for animations with a fixed timeline and predictable motion.

```vue
<motion.path
  :animate="{ pathLength: 1 }"
  :transition="{ duration: 2, type: 'tween' }"
/>
```

--------------------------------

### Animate Independent Transforms with Motion

Source: https://motion.dev/docs/improvements-to-the-web-animations-api-dx

Uses Motion's ability to animate individual transform properties like x and scaleX separately. This allows for more granular control and the ability to apply different animation options to each transform.

```javascript
animate(element, { x: 50, scaleX: 2 })
```

--------------------------------

### Stop Pointer Event Propagation with Capture Props

Source: https://motion.dev/docs/vue-gestures

Demonstrates how to prevent child elements from triggering parent motion component animations by using the @pointerDownCapture event handler with e.stopPropagation(). This prevents drag, tap gestures, and their associated while animations from firing on parent components.

```Vue
<motion.div :whilePress="{ scale: 2 }">
  <button @pointerDownCapture="e => e.stopPropagation()" />
</motion.div>
```

--------------------------------

### Detect Reduced Motion Preference in React with useReducedMotion Hook

Source: https://motion.dev/docs/react-accessibility

Illustrates how to use the `useReducedMotion` hook from Framer Motion to detect if a user has enabled the "Reduced Motion" setting. The hook returns a boolean value (`true` if reduced motion is enabled, `false` otherwise), which can be used for conditional logic in components.

```javascript
import { useReducedMotion } from "framer-motion"

// In your component
const shouldReduceMotion = useReducedMotion()
```

--------------------------------

### Nested AnimatePresence Default Behavior

Source: https://motion.dev/docs/react-animate-presence

Shows default behavior where nested AnimatePresence components prevent exit animations on inner children. Exit animations only fire on the outer AnimatePresence's direct children.

```jsx
<AnimatePresence>
  {show ? (
    <motion.section exit={{ opacity: 0 }}>
      <AnimatePresence>
        {/*
          * When `show` becomes `false`, exit animations
          * on these children will not fire.
          */}
        {children}
      </AnimatePresence>
    </motion.section>
  ) : null}
</AnimatePresence>
```

--------------------------------

### pause() Method

Source: https://motion.dev/docs/animate

Pauses the animation at its current position. The animation can be resumed later using the play() method without restarting from the beginning.

```APIDOC
## pause() Method

### Description
Pauses the animation until resumed with `play()`.

### Method
- **pause()** - Pauses animation at current time

### Usage Example
```javascript
const animation = animate(element, { opacity: 0 })
animation.pause()
```
```

--------------------------------

### Handle Press Cancel Events Outside Component

Source: https://motion.dev/docs/vue-motion-component

The onPressCancel callback fires when a pointer stops pressing and is released outside the component. Receives the triggering PointerEvent as an argument.

```vue
<motion.div @pressCancel="(event) => console.log(event)" />
```

--------------------------------

### Set `visualDuration` for spring animations in Motion.dev

Source: https://motion.dev/docs/animate

Shows how to use `visualDuration` to control the perceived duration of a spring animation. This option, set in seconds, ensures the bulk of the transition occurs within the specified time, making spring animations easier to coordinate visually.

```javascript
animate(
  "section",
  { rotateX: 90 },
  { type: "spring", visualDuration: 0.5, bounce: 0.25 }
)
```

--------------------------------

### ScrambleText Using Source Text Characters in React

Source: https://motion.dev/docs/react-scramble-text

Shows an advanced customization where the `ScrambleText` component is configured to only use characters that are present in the provided `text` content itself for the scrambling animation, by passing the `text` variable to the `chars` prop.

```jsx
<ScrambleText chars={text}>{text}</ScrambleText>
```

--------------------------------

### Render EasingCurve with bezier curve points

Source: https://motion.dev/docs/studio-sdk-easing-curve

Create a React component that renders an EasingCurve within an SVG element using an array of bezier curve control points. The curve prop accepts an array of four numeric values representing the cubic bezier curve coordinates.

```javascript
function Component() {
    return (
        <svg viewBox="0 0 100 100">
            <EasingCurve
                curve={[0.17, 0.67, 0.83, 0.67]}
                width={100}
                height={100}
            />
        </svg>
    )
}
```

--------------------------------

### Control Exit Animations with AnimatePresence `custom` Prop and Dynamic Variants (React)

Source: https://motion.dev/docs/react-animate-presence

When a component is removed from the React tree, its props can no longer be updated. The `custom` prop allows passing dynamic data to `AnimatePresence`'s children, which can then be used with Framer Motion's dynamic variants to alter exit animations based on this custom data.

```jsx
const variants = {
  hidden: (direction) => ({
    opacity: 0,
    x: direction === 1 ? -300 : 300
  }),
  visible: { opacity: 1, x: 0 }
}

export const Slideshow = ({ image, direction }) => (
  <AnimatePresence custom={direction}>
    <motion.img
      key={image.src}
      src={image.src}
      variants={variants}
      initial="hidden"
      animate="visible"
      exit="hidden"
    />
  </AnimatePresence>
)
```

--------------------------------

### Detect press on multiple elements with CSS selector

Source: https://motion.dev/docs/press

Use a CSS selector to attach press gesture listeners to multiple elements at once. The callback fires for each element that is pressed.

```javascript
press("a", () => console.log("link pressed"))
```

--------------------------------

### Propagate Exit Animations in Nested AnimatePresence (React)

Source: https://motion.dev/docs/react-animate-presence

Setting `propagate={true}` on a child `AnimatePresence` ensures that its exit animations are triggered when its parent `AnimatePresence` exits. This allows for coordinated exit animations across nested components.

```jsx
<AnimatePresence>
  {show ? (
    <motion.section exit={{ opacity: 0 }}>
      <AnimatePresence propagate>
        {/* This exit prop will now fire when show is false */}
        <motion.div exit={{ x: -100 }} />
      </AnimatePresence>
    </motion.section>
  ) : null}
</AnimatePresence>
```

--------------------------------

### Cancel a Motion `delay` operation

Source: https://motion.dev/docs/delay

The `delay` function returns another function that can be invoked to cancel the scheduled callback. This snippet illustrates how to store the cancellation function and use it to prevent the callback from ever executing.

```javascript
const cancel = delay(callback, 0.25)

cancel() // callback will never fire
```

--------------------------------

### Account for Page Scroll in Fixed Position Layout Animations with Motion.dev

Source: https://motion.dev/docs/vue-motion-component

Marks a `motion` component as a `position: fixed` element for layout animation purposes. This ensures that layout animations correctly account for page scroll when the component has a fixed position.

```html
<motion.div layoutRoot :style="{ position: 'fixed' }">
  <motion.div layout />
</motion.div>
```

--------------------------------

### Handle Hover End Event with `onHoverEnd` Callback in Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `onHoverEnd` callback function is invoked when a pointer stops hovering over the component. It provides the triggering `PointerEvent` object, allowing for custom hover-end logic.

```javascript
<motion.div onHoverEnd={(event) => console.log(event)} />
```

--------------------------------

### Customize Transform Order with `transformTemplate` in Motion.dev (Latest Values)

Source: https://motion.dev/docs/vue-motion-component

Allows customizing the order and composition of CSS transforms applied to a `motion` component. This function receives the latest transform values (e.g., `x`, `rotate`) and returns a custom transform string.

```html
<!-- // Use the latest transform values -->
<motion.div
  :style="{ x: 0, rotate: 180 }"
  :transformTemplate="({ x, rotate }) => `rotate(${rotate}deg) translateX(${x}px)`"
/>
```

--------------------------------

### duration Property

Source: https://motion.dev/docs/animate

Returns the duration of a single animation iteration without delay or repeat options. This property is read-only and cannot be modified after animation creation.

```APIDOC
## duration Property

### Description
Returns the duration of the animation. This is the duration of a single iteration of the animation, without delay or repeat options. It is **read-only**.

### Property
- **duration** (number) - Read-only - Duration in seconds of a single animation iteration

### Usage Example
```javascript
const animation = animate(element, { opacity: 0 })

const duration = animation.duration
console.log(duration) // Returns duration value
```
```

--------------------------------

### Enable Layout Animations within Scrollable Elements in Motion.dev

Source: https://motion.dev/docs/vue-motion-component

Indicates that a scrollable ancestor element should be measured for layout animations. This prop ensures `motion` components correctly animate within scroll containers by accounting for their scroll offset.

```html
<motion.div layoutScroll style="{ overflow: 'scroll' }">
  <motion.div layout />
</motion.div>
```

--------------------------------

### Use transformValue with styleEffect for computed styles

Source: https://motion.dev/docs/style-effect

Combine transformValue with styleEffect to apply computed or transformed motion values to CSS properties. This enables complex style calculations based on motion value outputs.

```javascript
const blur = motionValue(2)
const filter = transformValue(() => `blur(${blur.get()}px)`)

styleEffect("img", { filter })
```

--------------------------------

### Handle onDirectionLock callback

Source: https://motion.dev/docs/react-motion-component

Callback function that fires when a drag direction is determined after dragDirectionLock is enabled. Receives the locked axis as a parameter.

```JSX
<motion.div
  drag
  dragDirectionLock
  onDirectionLock={axis => console.log(axis)}
/>
```

--------------------------------

### Destroy Motion Value and Clean Up Subscribers

Source: https://motion.dev/docs/vue-motion-value

Clean up and destroy a motion value along with all its subscribers using the destroy method. Normally handled automatically, but necessary for manually created motion values outside the Vue render cycle.

```javascript
x.destroy()
```

--------------------------------

### Function: glide()

Source: https://motion.dev/docs/glide

Animates transforms using momentum physics. This function is deprecated; use `type: "inertia"` with the new `animate()` function. It simulates momentum, overriding target keyframes and duration.

```APIDOC
## FUNCTION glide()

### Description
Animates transforms using momentum physics, ideal for creating scroll momentum animations. This function is **deprecated**. You can use `type: "inertia"` with the new `animate()` function. `glide` is a simulation, so provided target keyframes and `duration` will be overridden.

### Parameters
- **velocity** (number) - Optional - Default: `0` or the value's current velocity. The velocity (in units per second) at which to start the glide animation.
- **power** (number) - Optional - Default: `0.8`. Influences how much of the initial `velocity` is factored into the animation, and thus how far the animation will glide. Higher values will throw the animation further and feel lighter, whereas lower values will feel heavier.
- **decay** (number) - Optional - Default: `0.325`. A time constant (in seconds) used to calculate velocity decay. Higher values lead to longer animations with more gradual deceleration and a lighter feel.
- **restSpeed** (number) - Optional - Default: `2`, or `0.05` for `scale`. A speed (in absolute units per second) below which the spring animation is considered finished.
- **restDistance** (number) - Optional - Default: `0.5` or `0.01` for `scale`. A distance from the animation target, below which the spring animation is considered finished.
- **changeTarget** (function) - Optional - A function that takes the calculated target and returns a new one. For instance, the function in the following example will snap the target to the next `100`.
- **min** (number) - Optional - A minimum boundary for the glide animation. If the animated value exceeds this boundary, a spring animation will take over to snap the value to `min`.
- **max** (number) - Optional - A maximum boundary for the glide animation. If the animated value exceeds this boundary, a spring animation will take over to snap the value to `max`.
- **bounceStiffness** (number) - Optional - Default: `100`. The attraction force of a spring used if the animation exceeds the boundaries defined by `min`/`max`. Higher values create faster, sharper movement.
- **bounceDamping** (number) - Optional - Default: `10`. The opposing force of a spring. Higher values reduce the bounciness of the spring.

### Usage Examples
```javascript
import { animate, glide } from "motion"

// Basic usage
animate(
  element,
  { x: 500 },
  { easing: glide() }
)

// Overriding velocity
animate(
  "#carousel",
  { x: 100 },
  { easing: glide({ velocity: 1000 }) }
)

// Value-specific options (combining glide and spring)
animate(
  "#ball",
  { x: 0, y: 0 },
  {
    x: { easing: glide({ velocity: 200 }) },
    y: { easing: spring({ velocity: 500 }) }
  }
)

// Setting boundaries
glide({ min: -100, max: 100 })

// Overriding power
glide({ power: 1 })

// Overriding decay
glide({ decay: 0.5 })

// Overriding restSpeed (example shown with spring, but applicable to glide's internal spring)
spring({ restSpeed: 1 })

// Overriding restDistance (example shown with spring, but applicable to glide's internal spring)
spring({ restDistance: 0.1 })

// Using changeTarget
const roundTo = 100
glide({
  changeTarget: (target) => Math.ceil(target / roundTo) * roundTo
})

// Setting min boundary
glide({ min: -100 })

// Setting max boundary
glide({ max: 100 })

// Custom bounce stiffness
glide({ min: 100, bounceStiffness: 500 })

// Custom bounce damping
glide({ max: 100, bounceDamping: 30 })
```

### Notes
`glide` will automatically pass velocity from any running animations into the next one, so interrupting an animation will feel natural. This can be overridden by manually passing `velocity`.

There are currently some limitations with the `spring` easing (which is used for boundary bounces):
- **Duration**: Springs with `damping: 0` can last an infinite amount of time, but the Web Animations API needs a finite `duration`. Springs currently max out at 10 seconds (which is more than long enough for the vast majority of UI animations). Increase `damping` relative to `stiffness` to decrease the duration of your animation.
- **Timeline keyframes**: `spring` is supported in `timeline` but independent transforms **must** be defined with start and end keyframes: `{ x: [0, 100] }`.
- **No hardware acceleration**: `spring` only works with independent transforms, which are not yet hardware accelerated in browsers.
```

--------------------------------

### Set Typewriter Typing Speed Variance to 0.5 in React

Source: https://motion.dev/docs/react-typewriter

Applies a `0.5` factor to the typing speed, introducing a moderate level of natural variance. This helps emulate human typing behavior more closely by creating a range of speeds.

```jsx
<Typewriter variance={0.5}>Hello world!</Typewriter>
```

--------------------------------

### Detect successful press completion

Source: https://motion.dev/docs/press

Use the info parameter in the press end callback to determine if the press was successful. The success property is true for completed clicks and false for presses that ended outside the element.

```javascript
press(element, () => {
  return (endEvent, info) => {
    console.log("press ", info.success ? "end" : "cancel")
  }
})
```

--------------------------------

### onViewportLeave - Viewport Exit Callback

Source: https://motion.dev/docs/react-motion-component

Callback function triggered when an element leaves the viewport. Receives IntersectionObserverEntry object with intersection event details including intersectionRect coordinates.

```jsx
<motion.div onViewportLeave={(entry) => console.log(entry.intersectionRect)} />
```

--------------------------------

### Animate SVG Filters Using Parent Variants

Source: https://motion.dev/docs/vue-gestures

Shows how to work around the limitation that SVG filter elements don't receive gesture events by applying while- props and event handlers to the parent SVG element and using variants to animate child filter components. This allows hover animations on feGaussianBlur and other filter elements.

```Vue
<template>
    <motion.svg whileHover="hover">
      <filter id="blur">
        <motion.feGaussianBlur
          :stdDeviation="0"
          :variants="{ hover: { stdDeviation: 2 } }"
        />
      </filter>
    </motion.svg>
</template>
```

--------------------------------

### animate() - Motion Values Animation (Hybrid)

Source: https://motion.dev/docs/animate

Animate React motion values directly. The animate() function automatically updates motion values with the latest animation values.

```APIDOC
## animate() - Motion Values

### Description
Animate React motion values, which are automatically updated with the latest animation values. Available in the hybrid version.

### Syntax
```javascript
const motionValue = motionValue(initialValue)
animate(motionValue, targetValue, options?)
```

### Parameters
- **motionValue** (MotionValue) - Required - Motion value to animate
- **targetValue** (number | string | object) - Required - Target animation value
- **options** (object) - Optional - Animation configuration

### Request Example
```javascript
const x = motionValue(0)
animate(x, 200, { duration: 0.5 })
```

### Notes
Motion values are automatically updated with the latest values during animation, making them ideal for React component integration.
```

--------------------------------

### Set animation `duration` option in Motion.dev

Source: https://motion.dev/docs/animate

Illustrates how to specify the `duration` of an animation. This option controls how long the animation takes to complete and can also be used for spring animations when `bounce` is set.

```javascript
animate("ul > li", { opacity: 1 }, { duration: 1 })
```

--------------------------------

### Detect hover using CSS selector with Motion

Source: https://motion.dev/docs/hover

Attach hover gesture listeners to multiple elements matching a CSS selector. The callback fires for each element that receives a hover gesture.

```javascript
hover("a", () => console.log("link hovered"))
```

--------------------------------

### Detect drag gesture end with onDragEnd callback

Source: https://motion.dev/docs/vue-motion-component

The onDragEnd callback fires when a drag gesture completes. It receives the triggering PointerEvent and info object containing final delta, offset, point, and velocity values.

```vue
<motion.div drag @dragEnd="(event, info) => console.log(info.delta.x)" />
```

--------------------------------

### Cancel propEffect with Cleanup Function

Source: https://motion.dev/docs/prop-effect

propEffect returns a cleanup function that stops applying motion value changes to the target object when called. This is useful for cleanup in component lifecycles or when the effect is no longer needed.

```javascript
const rotateX = motionValue(0)
const cancel = propEffect(threeRotation, { x: rotateX })

cancel()
```

--------------------------------

### Use Motion Values for Performance Optimization

Source: https://motion.dev/docs/vue-motion-component

Use useMotionValue hook to animate values outside the Vue render cycle, avoiding unnecessary re-renders. Motion values update the DOM directly without triggering Vue's reactivity system, improving performance for frequent animations.

```vue
<script setup>
  import { useMotionValue } from "motion-v"
  
  const x = useMotionValue(0)
  let timeout;
  
  onMounted(() => {
    timeout = setTimeout(() => x.set(100), 1000)
  })
  
  onUnMounted(()=>{
    clearTimeout(timeout)
  })
</script>

<template>  
   <motion.div :style="{ x }" />
</template>
```

--------------------------------

### Exit animations with v-if conditional rendering

Source: https://motion.dev/docs/vue-animate-presence

AnimatePresence detects when direct children are removed from the Vue tree due to v-if conditions. The component will animate out before being removed from the DOM.

```vue
<AnimatePresence>
  <Modal v-if="show" key="modal" />
</AnimatePresence>
```

--------------------------------

### Control Ticker Speed with Velocity - React

Source: https://motion.dev/docs/react-ticker

Adjusts the ticker animation speed using the velocity prop, which accepts pixels per second. Positive values scroll forward, negative values reverse direction, and zero stops the animation.

```jsx
<Ticker items={items} velocity={100} />
```

```jsx
<Ticker items={items} velocity={-100} />
```

```jsx
<Ticker items={items} velocity={0} />
```

--------------------------------

### Correcting `borderRadius` and `boxShadow` Distortion in Motion

Source: https://motion.dev/docs/vue-layout-animations

When animating with `motion`, `scale` can distort `borderRadius` and `boxShadow`. Motion automatically corrects this distortion if these properties are set via the `style` prop, either directly or as motion values. This ensures visual integrity during layout animations.

```JSX
<motion.div layout :style="{ borderRadius: 20 }" />
```

--------------------------------

### Configure dragConstraints with pixel values in Motion Vue

Source: https://motion.dev/docs/vue-motion-component

Set drag constraints as an object with optional top, left, right, and bottom pixel values to limit draggable area movement. Alternatively, pass a ref to another element to use its bounding box as constraints.

```vue
<motion.div
  drag="x"
  :dragConstraints="{ left: 0, right: 300 }"
/>
```

```vue
<script setup>
  import { useDomRef } from "motion-v"
  const constraintsRef = useDomRef()
</script>
<template>
  <motion.div ref="constraintsRef">
    <motion.div drag :dragConstraints="constraintsRef" />
  </motion.div>
</template>
```

--------------------------------

### Stop Animation with Motion

Source: https://motion.dev/docs/improvements-to-the-web-animations-api-dx

Uses Motion's stop() method to cancel an animation while preserving the element's current state. Unlike cancel(), the element remains at its position when the animation stops.

```javascript
const animation = animate(element, { opacity: 0 }, { duration: 1000 })
setTimeout(() => { animation.stop()}, 500)
```

--------------------------------

### Handle Pan Gesture with `@pan` Event in Vue

Source: https://motion.dev/docs/vue-gestures

This snippet shows how to use the `@pan` event listener on a `motion.div` component. The pan gesture detects when a pointer presses down and moves more than 3 pixels, ending upon pointer release. The event callback receives the event object and point information.

```html
<motion.div @pan="(e, pointInfo) => {}" />
```

--------------------------------

### propagate (Gestures)

Source: https://motion.dev/docs/react-motion-component

Prevents child gestures from propagating to their parent components. Currently supports `tap` gestures.

```APIDOC
## propagate

### Description
Prevent children gestures from propagating to their parents. Currently only supports `tap`.

### Type
`object`

### Parameters
- **tap** (boolean) - If `false`, prevents tap gestures from propagating to parent components.

### Usage Example
```jsx
<motion.div whileTap={{ scale: 2 }}>
  // Pressing this button won't fire the above scale animation
  <motion.button
    whileTap={{ opacity: 0.8 }}
    propagate={{ tap: false }}
  />
</motion.div>
```
```

--------------------------------

### Control dragMomentum for pan gesture momentum

Source: https://motion.dev/docs/vue-motion-component

Enable or disable momentum application from the pan gesture when dragging finishes. Default is true. Set to false to prevent momentum-based animation after drag release.

```vue
<motion.div
  drag
  :dragConstraints="{ left: 0, right: 300 }"
  :dragMomentum="false"
/>
```

--------------------------------

### onDirectionLock

Source: https://motion.dev/docs/react-motion-component

Callback function that fires when a drag direction (x or y) is determined and locked.

```APIDOC
## onDirectionLock

### Description
Callback function that fires a drag direction is determined.

### Type
`(axis: "x" | "y") => void`

### Parameters
- **axis** (string) - The determined axis of drag, either `"x"` or `"y"`.

### Usage Example
```jsx
<motion.div
  drag
  dragDirectionLock
  onDirectionLock={axis => console.log(axis)}
/>
```
```

--------------------------------

### Cancel Animation with WAAPI

Source: https://motion.dev/docs/improvements-to-the-web-animations-api-dx

Demonstrates using WAAPI's cancel() method to stop an animation and remove it completely as if it never played. The animation is stopped and the element returns to its original state.

```javascript
const animation = element.animate({ opacity: 0 }, { duration: 1000 })
setTimeout(() => { animation.cancel()}, 500)
```

--------------------------------

### dragMomentum

Source: https://motion.dev/docs/react-motion-component

Determines whether momentum from the pan gesture is applied to the component when dragging finishes.

```APIDOC
## dragMomentum

### Description
Apply momentum from the pan gesture to the component when dragging finishes.

### Type
`boolean`

### Default
`true`

### Usage Example
```jsx
<motion.div
  drag
  dragConstraints={{ left: 0, right: 300 }}
  dragMomentum={false}
/>
```
```

--------------------------------

### Use EasingCurve with easing function

Source: https://motion.dev/docs/studio-sdk-easing-curve

Pass an easing function from the motion library directly to the EasingCurve component's curve prop instead of an array of bezier points. This allows you to visualize predefined easing functions.

```javascript
import { circIn } from "motion"

<EasingCurve curve={circIn} />
```

--------------------------------

### Stopping an Animation and Committing Styles (JavaScript)

Source: https://motion.dev/docs/animate

The `stop()` method halts the animation and commits any currently animated values to the element's inline styles. Once stopped, an animation cannot be restarted.

```javascript
const animation = animate(element, { opacity: 0 })
animation.stop()
```

--------------------------------

### Enable Dragging with `drag` Prop in Framer Motion

Source: https://motion.dev/docs/react-motion-component

The `drag` prop enables dragging functionality for a `motion` component. Set to `true` for dragging in both X and Y directions, or to `'x'` or `'y'` to restrict dragging to a single axis.

```javascript
<motion.div drag />
```

--------------------------------

### Apply propEffect to Three.js Mesh Position

Source: https://motion.dev/docs/prop-effect

propEffect can be used with Three.js objects to bind motion values to mesh properties like position. This enables smooth animations of 3D object properties synchronized with the animation frame loop.

```javascript
const cube = new THREE.Mesh(geometry, material)
const x = motionValue(0)

propEffect(cube.position, { x })
```

--------------------------------

### Update MotionValues to trigger `svgEffect` re-render (JavaScript)

Source: https://motion.dev/docs/svg-effect

This snippet shows how changes to `motionValue` instances, whether through direct `set` calls or animation functions like `animate`, automatically trigger `svgEffect` to re-render the associated SVG element. The element updates on the next animation frame, reflecting the new motion value.

```JavaScript
stroke.set("#f00")
animate(strokeWidth, 1)
```

--------------------------------

### Interrupt Animation with Motion

Source: https://motion.dev/docs/improvements-to-the-web-animations-api-dx

Shows Motion's automatic interruption of existing animations when new values are passed to animate(). Motion smoothly transitions to the new target without jumping back to the old animation.

```javascript
animate(
  element,
  { transform: "translateX(300px)" },
  { duration: 2, iterations: Infinity }
)
  
setTimeout(() => {
  animate(element, { transform: "none" }, { duration: 500 })
}, 500)
```

--------------------------------

### Fixing Layout Animations: Set Parent `position` for `mode="popLayout"` in Vue

Source: https://motion.dev/docs/vue-animate-presence

When using `mode="popLayout"`, elements are absolutely positioned. To prevent unexpected positioning due to active `transform` on parents, ensure the animating parent has a non-static `position`, such as `relative`.

```html
<motion.ul layout :style="{ position: 'relative' }">
  <AnimatePresence mode="popLayout">
      <motion.li v-for="item in items" layout :key="item.id" />
  </AnimatePresence>
</motion.ul>
```

--------------------------------

### Enable axis lines on EasingCurve

Source: https://motion.dev/docs/studio-sdk-easing-curve

Display axis reference lines on the easing curve by setting the axisWidth prop for line thickness and axisColor prop for the line color. Axis lines are not rendered by default.

```javascript
<EasingCurve curve={curve} axisWidth={3} axisColor="#333" />
```

--------------------------------

### Detect press on specific element by ID

Source: https://motion.dev/docs/press

Attach a press gesture listener to a specific element using getElementById. The callback fires when the element is pressed.

```javascript
press(
  document.getElementById("my-id"),
  () => {
    console.log("my-id pressed!")
  }
)
```

--------------------------------

### Animating a Motion Value with automatic animation termination in JavaScript

Source: https://motion.dev/docs/motion-value

This snippet illustrates how `motionValue` automatically handles concurrent animations. When a new `animate` call is made on the same `motionValue` while another animation is active, the existing animation is automatically stopped before the new one begins, preventing conflicts.

```javascript
const color = motionValue("#f00")

animate(color, "#0f0")

animate(color, "#333") // Will automatically end the existing animation
```

--------------------------------

### Adjust Time Constant for Inertia Animation in Framer Motion

Source: https://motion.dev/docs/vue-transitions

Modifies the duration of the deceleration phase in an inertia animation. Changing this value affects the overall feel and speed of the animation's slowdown. Default is 700.

```Framer Motion
<motion.div
  drag
  :dragTransition="{ timeConstant: 200 }"
/>
```

--------------------------------

### Cancelling an Animation (JavaScript)

Source: https://motion.dev/docs/animate

The `cancel()` method stops the animation and reverts the animated element to its initial state before the animation began. This effectively undoes the animation's effects.

```javascript
const animation = animate(element, { opacity: 0 })
animation.cancel()
```

--------------------------------

### Pausing an Animation (JavaScript)

Source: https://motion.dev/docs/animate

The `pause()` method halts the animation at its current state. The animation will remain paused until explicitly resumed with the `play()` method.

```javascript
const animation = animate(element, { opacity: 0 })
animation.pause()
```

--------------------------------

### Prevent child gesture propagation with propagate

Source: https://motion.dev/docs/react-motion-component

Prevents child component gestures from propagating to parent components. Currently supports tap gesture. Set propagate={{ tap: false }} on child elements to block tap animation propagation.

```JSX
<motion.div whileTap={{ scale: 2 }}>
  <motion.button
    whileTap={{ opacity: 0.8 }}
    propagate={{ tap: false }}
  />
</motion.div>
```

--------------------------------

### Stop and cancel drag gestures manually

Source: https://motion.dev/docs/react-use-drag-controls

End a drag gesture programmatically using stop() to trigger onDragEnd callback, or cancel() to skip the callback. Gestures automatically stop on pointerup events.

```javascript
controls.stop()
// or
controls.cancel()
```

--------------------------------

### Enable dragDirectionLock for single-axis dragging

Source: https://motion.dev/docs/react-motion-component

Locks the drag direction to the first detected axis (x or y) based on initial movement. Once locked, the component will only drag along that axis for the remainder of the gesture. Default is false.

```JSX
<motion.div drag dragDirectionLock />
```

--------------------------------

### Detect drag direction lock with onDirectionLock callback

Source: https://motion.dev/docs/vue-motion-component

The onDirectionLock callback fires when a drag direction is determined (x or y axis). Used with dragDirectionLock to identify which axis the drag gesture is constrained to.

```vue
<motion.div
  drag
  dragDirectionLock
  @directionLock="axis => console.log(axis)"
/>
```

--------------------------------

### Control dragMomentum on drag release

Source: https://motion.dev/docs/react-motion-component

Determines whether momentum from the pan gesture is applied to the component when dragging finishes. Enabled by default (true). Set to false to disable momentum-based animation.

```JSX
<motion.div
  drag
  dragConstraints={{ left: 0, right: 300 }}
  dragMomentum={false}
/>
```

--------------------------------

### dragDirectionLock

Source: https://motion.dev/docs/react-motion-component

Locks the drag direction into the soonest detected axis (x or y) for the remainder of the gesture.

```APIDOC
## dragDirectionLock

### Description
Locks drag direction into the soonest detected direction. For example, if the component is moved more on the `x` axis than `y` axis before the drag gesture kicks in, it will **only** drag on the `x` axis for the remainder of the gesture.

### Type
`boolean`

### Default
`false`

### Usage Example
```jsx
<motion.div drag dragDirectionLock />
```
```

--------------------------------

### React Component: EasingCurve

Source: https://motion.dev/docs/studio-sdk-easing-curve

The EasingCurve component is a React component that renders a cubic bezier easing curve or easing function as an SVG path. It supports axis lines and customisable styling, allowing for visual representation of animation easing.

```APIDOC
## Component: EasingCurve

### Description
`EasingCurve` is a React component that renders a cubic bezier easing curve or easing function as an SVG path. It supports axis lines and customisable styling.

### Type
React Component

### Import
```javascript
import { EasingCurve } from "motion-studio"
```

### Props
#### `curve`
- **Type**: `array` or `function`
- **Required**: Yes
- **Description**: Defines the easing curve. Can be an array of valid bezier curve points (e.g., `[0.17, 0.67, 0.83, 0.67]`) or an easing function (e.g., `circIn` from `motion`).

#### Layout Props (`width`, `height`, `top`, `left`)
- **Type**: `number` (pixels)
- **Required**: No
- **Description**: Used for sizing and positioning the curve within its container. While `width` and `height` can differ, a square aspect ratio is recommended for visual clarity.
    - `width`: (number) - Optional - The width of the curve's drawing area.
    - `height`: (number) - Optional - The height of the curve's drawing area.
    - `top`: (number) - Optional - The top offset for positioning the curve.
    - `left`: (number) - Optional - The left offset for positioning the curve.

#### Line Styling Props (`color`, `pathWidth`)
- **Type**: `string` for `color`, `number` for `pathWidth`
- **Required**: No
- **Description**: Customizes the appearance of the drawn easing curve line.
    - `color`: (string) - Optional - The color of the curve line (e.g., `"#fff"`).
    - `pathWidth`: (number) - Optional - The stroke width of the curve line (e.g., `2`).

#### Axis Styling Props (`axisWidth`, `axisColor`)
- **Type**: `number` for `axisWidth`, `string` for `axisColor`
- **Required**: No (axis lines are not drawn by default)
- **Description**: Configures the drawing and styling of optional axis lines.
    - `axisWidth`: (number) - Optional - The stroke width of the axis lines (e.g., `3`). If defined, axis lines will be drawn.
    - `axisColor`: (string) - Optional - The color of the axis lines (e.g., `"#333"`).

#### `transition`
- **Type**: `object`
- **Required**: No
- **Description**: Enables smooth transitions between different easing curves when the `curve` prop changes. Useful for animating between preset curves.
    - Example: `{ duration: 0.3 }`

### Usage Example
```javascript
import React from "react";
import { EasingCurve } from "motion-studio";
// import { circIn } from "motion"; // For easing functions

function MyComponent() {
    const bezierCurvePoints = [0.17, 0.67, 0.83, 0.67]; // Example cubic bezier points
    // const easingFunction = circIn; // Example easing function

    return (
        <svg viewBox="0 0 100 100" width="100" height="100">
            <EasingCurve
                curve={bezierCurvePoints} // Or curve={easingFunction}
                width={100}
                height={100}
                top={0}
                left={0}
                color="#007bff"
                pathWidth={2}
                axisWidth={1}
                axisColor="#cccccc"
                transition={{ duration: 0.5, ease: "easeInOut" }}
            />
        </svg>
    );
}

export default MyComponent;
```

### Renders
The component renders an `<svg>` `<path />` element representing the easing curve. If `axisWidth` is provided, it also renders a `<polyline />` component for the axis lines within the SVG.
```

--------------------------------

### Adjust Typewriter Typing Speed in React

Source: https://motion.dev/docs/react-typewriter

Sets the typing speed of the `Typewriter` component to a predefined value like 'slow'. Other options include 'fast' or a custom numeric interval in milliseconds for fine-grained control.

```jsx
<Typewriter speed="slow">Hello world!</Typewriter>
```

--------------------------------

### Cancel `svgEffect` application with cleanup function (JavaScript)

Source: https://motion.dev/docs/svg-effect

`svgEffect` returns a cleanup function that, when invoked, stops the effect from applying further changes to the motion values on the element. This is crucial for managing resources and preventing memory leaks when an SVG animation is no longer needed.

```JavaScript
const width = motionValue("0px")
const cancel = svgEffect("#progress", { width })

cancel()
```

--------------------------------

### Animate `borderRadius` Directly (Less Performant) in JavaScript

Source: https://motion.dev/docs/performance

This JavaScript snippet shows animating the `borderRadius` property directly. Similar to `boxShadow`, animating `borderRadius` can be less performant as it often triggers expensive paint operations, which can negatively impact animation smoothness.

```javascript
// ❌
animate(element, { borderRadius: "50px" })
```

--------------------------------

### Cancel hover gesture detection with Motion

Source: https://motion.dev/docs/hover

The hover function returns a cancel function that removes all active event handlers associated with the gesture when called.

```javascript
const cancelHover = hover(element, callback)

cancelHover()
```

--------------------------------

### Cancel styleEffect to stop applying style updates

Source: https://motion.dev/docs/style-effect

styleEffect returns a cleanup function that stops applying motion value changes to the element when called. Use this to remove style bindings and prevent memory leaks.

```javascript
const width = motionValue("0px")
const cancel = styleEffect("#progress", { width })

cancel()
```

--------------------------------

### Apply Drag Constraints to a Single Axis in Vue

Source: https://motion.dev/docs/vue-gestures

This snippet shows how to constrain the drag movement of a `motion.div` component to a single axis ('x' in this case) and within specific pixel boundaries. The `dragConstraints` prop defines the `left` and `right` limits for horizontal movement.

```html
<motion.div
  drag="x"
  :dragConstraints="{ left: 0, right: 300 }"
/>
```

--------------------------------

### Stop Active Motion Value Animation

Source: https://motion.dev/docs/vue-motion-value

Halt the currently active animation on a motion value using the stop method. Immediately stops animation without resetting velocity or breaking continuity.

```javascript
x.stop()
```

--------------------------------

### Override SVG `transformBox` for custom transform origin with `svgEffect` (JavaScript)

Source: https://motion.dev/docs/svg-effect

By default, `svgEffect` applies `transform-box: fill-box` for CSS-like transform origins. This snippet demonstrates how to manually override this behavior by setting `transformBox` to a custom `motionValue`, allowing for specific control over the SVG transform origin, such as `view-box`.

```JavaScript
svgEffect("path", { transformBox: motionValue("view-box") })
```

--------------------------------

### Vertical Ticker Animation - React

Source: https://motion.dev/docs/react-ticker

Configures the Ticker component to scroll vertically instead of the default horizontal direction using the axis prop set to 'y'.

```jsx
<Ticker items={items} axis="y" />
```

--------------------------------

### Set Typewriter Typing Speed Variance to Zero in React

Source: https://motion.dev/docs/react-typewriter

Disables natural typing speed variance by setting the `variance` prop to `0`. This ensures a consistent, non-varying typing speed for all characters.

```jsx
<Typewriter variance={0}>Hello world!</Typewriter>
```

--------------------------------

### Conditionally Disable Parallax Animation in React

Source: https://motion.dev/docs/react-accessibility

Shows how to conditionally apply a parallax effect based on the `shouldReduceMotion` state. By setting the `y` position to `0` when reduced motion is enabled, the parallax scrolling effect is disabled, preventing potential discomfort for users pre-disposed to motion sickness.

```javascript
function Parallax() {
  const shouldReduceMotion = useReducedMotion()
  const { scrollY } = useScroll()

  const y = useTransform(scrollY, [0, 1], [0, -0.2], {
    clamp: false,
  })

  return (
    <motion.div style={{ y: shouldReduceMotion ? 0 : y }} />
  )
}
```

--------------------------------

### Cancel active press gesture

Source: https://motion.dev/docs/press

The press function returns a cancel function that removes all active event handlers for the gesture. Call this function to programmatically cancel the press.

```javascript
const cancelPress = press(element, callback)

cancelPress()
```

=== COMPLETE CONTENT === This response contains all available snippets from this library. No additional content exists. Do not make further requests.
