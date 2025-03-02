## Pygame: Drawing Text with a Function

### Overview

As part of this activity, you'll learn:

1. how to write a Python function for drawing text onto your Pygame window.
2. which parameters your `draw_text()` function can take (some are required, others optional)

---

### What does Pygame need to know to draw text onto your screen?

**Required info:**

In no particular order:

- **text**: What text or message to display
- **x** and **y coordinates**: For top, left corner of the rectangle containing your text/message
- **font size**: Self-explanatory
- **color**: Self-explanatory
- **surface**: Where should Pygame draw the text? (on the **screen** you defined in your code)
```python
screen = pygame.display.set_mode((config.WINDOW_WIDTH, config.WINDOW_HEIGHT))
```

**Optional info:**

- **font name**: For example: Arial, Times New Roman, Courier New
- Setting the `font_name` parameter to `None` tells Pygame to use the default font on your computer
```python
font_name=None # No quotes around the value None
```
---
```python
# Set up the font
font = pygame.font.Font("Courier New.ttf", size)  # Using a True Type Font (.ttf) file, i.e., a custom font file
# or
font = pygame.font.SysFont("Courier New", size)  # Using a system font (Courier New)
```
- **font styling**: Should the font be bolded or italicized?
    - Use the **bold** or **italic** parameter
    - Either parameter can be set to True or False
        - Example: Setting the bold parameter to `True` will bold your text
        - Example: Setting the italic parameter to `False` means you don't want your text to be italicized
---

