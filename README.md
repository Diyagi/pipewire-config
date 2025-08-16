This is my overly complicated and perhaps unnecessary PipeWire setup. My goal was to mimic somewhat what I had going in Windows with VoiceMeeter Potato.

A couple of things for me to remember:
- Pipewire and pipewire-pulse are different things with different configs, trying to config an stream that was created by pipewire-pulse using an pipewire config wont work.
- Wireplumber will try to target default devices unless it finds the property `target.object` in the stream/device properties, in which case wireplumber will try to target the value of that prop.
