# Fluid Video

To achieve fluid video, apply this CSS hack:
```css
  .video-wrapper {
    height: 0;
    padding-bottom: 56.25% /* 16 : 9 */
  }
  
  video {
    width: 100%;
    height: auto;
  }
```

The same can be achieved for wrapper in iframe
