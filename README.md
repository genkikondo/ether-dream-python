# Ether Dream for Python

Example:

```python
import ether_dream


class PointStream:
    def __iter__(self):
        return self

    def __next__(self):
        return (0, 0, 65535, 65535, 65535)


d = ether_dream.get_dac()
d.play_point_stream(iter(PointStream()))
```
