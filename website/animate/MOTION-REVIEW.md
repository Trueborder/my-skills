# Review web UI motion

Record the trigger, frequency and purpose. Inspect the actual interaction where possible. Exercise quick open/close, repeated input, the exit path, keyboard focus and reduced motion before passing the change. Keep the UI operable while transitions run, including when a transition is interrupted or skipped.

- Make frequent actions immediate. Keep an occasional state change only if it adds feedback or helps the user follow where content moved.
- Use the existing timing and easing tokens. Confirm the visual starting point and transform origin, especially for anchored popovers. Check entrance and exit separately.
- Reverse or retarget toggles and notices from their current state. Avoid keyframes that restart on repeated input. Verify that cancelled callbacks and overlapping interactions cannot leave stale content or focus behind.
- Name the properties being animated. Profile a repeated or visibly costly effect using available browser tooling. Verify hover capability and reduced-motion behavior.
- For each finding, give the affected interaction, evidence, user impact and smallest correction. Separate a proposal for new motion from a bug in existing motion.

## Direct manipulation

Track the pointer from its initial offset. Avoid easing position while the pointer is down. Capture the pointer where needed and clear the gesture on cancellation or loss of capture. Preserve page scroll on axes that the component does not own.

On release, estimate velocity from recent position and time samples. Start settling from the current rendered position and pass release velocity to the spring using its expected units. Let a fast flick or sufficient distance reach the intended destination. Keep a visible way to reverse or dismiss the interaction, and supply equivalent keyboard controls.

Use critically damped settling as the default. Reserve overshoot or elastic edges for a gesture whose momentum benefits from visible feedback. Check grabbing an element again while it is settling and test the reduced-motion path.

Adapted from the local versions of Emil Kowalski's `emil-design-eng`, `review-animations`, `find-animation-opportunities` and `apple-design`.
