# Image Layers / Caching
- Layer based architecture
- Each instruction represents a layer in a dockerfile
- If we build an image, that has previously been built, we only need to rebuild the changed layers
- Whenever a layer is changed, all the following layers must be rebuilt (including the changed layer)