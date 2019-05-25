+++
# Slider widget.
widget = "slider"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 1  # Order that this section will appear.

# Slide interval.
# Use `false` to disable animation or enter a time in ms, e.g. `4000` (5s).
interval = false

# Slide height (optional).
# E.g. `500px` for 500 pixels or `calc(100vh - 70px)` for full screen.
height = ""

# Slides.
# Duplicate an `[[item]]` block to add more slides.
[[item]]
  title = "the Dyer Laboratory"
  content = "Population & Landscape Genetics"
  align = "center"  # Choose `center`, `left`, or `right`.

  # Overlay a color or image (optional).
  #   Deactivate an option by commenting out the line, prefixing it with `#`.
  overlay_color = "#666"  # An HTML color value.
  overlay_img = "headers/book.jpg"  # Image path relative to your `static/img/` folder.
  overlay_filter = 0.25  # Darken the image. Value in range 0-1.

  # Call to action button (optional).
  #   Activate the button by specifying a URL and button label below.
  #   Deactivate by commenting out parameters, prefixing lines with `#`.
  # cta_label = "Get Academic"
  # cta_url = "https://sourcethemes.com/academic/"
  # cta_icon_pack = "fas"
  # cta_icon = "graduation-cap"

[[item]]
  title = "Dyerlab"
  content = "Microevolution"
  align = "left"

  #overlay_color = "#fff"  # An HTML color value.
  overlay_img = "headers/rice-forest.jpg"  # Image path relative to your `static/img/` folder.
  overlay_filter = 0.15  # Darken the image. Value in range 0-1.
  
[[item]]
  title = "the Dyerlab"
  content = "Theory & tool design"
  align = "center"

  #overlay_color = "#ccc"  # An HTML color value.
  overlay_img = "headers/whiteboard.jpg"  # Image path relative to your `static/img/` folder.
  overlay_filter = 0.45  # Darken the image. Value in range 0-1.

[[item]]
  title = "Dyerlab"
  content = "Pollen-mediated gene flow"
  align = "right"

  overlay_color = "#333"  # An HTML color value.
  overlay_img = "headers/dogwood-flower.jpg"  # Image path relative to your `static/img/` folder.
  overlay_filter = 0.05  # Darken the image. Value in range 0-1.
+++
