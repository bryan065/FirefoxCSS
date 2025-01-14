Changes:
- Light/dark theme support
- Rounded corners (including browser content window)
- Identity badge colors
- Floating link popup, rounded corners
- Context menu theming, also removed unused entries (personalized to me)
- Expand vertical tabs on hover (using Firefox's built in vertical tabs)
- Hide Specific toolbar buttons (personalized to me)

To-Do:

- [ ] Adjust shadow darnkess/colors in light theme
- [ ] Find a way to keep the Firefox vertical tabs always expanded (Will randomly revert to compact mode)
- [ ] Find a way to restore drop shadows under sidebar and browser content windows.
  - Currently, the side bar must have `z-index:4` in order to maintain proper animations with my CSS. However, this places it above the sidebar and brower content window.
  - This will cut off any shadows that go under the vertical tabs bar (aka, any shadows to the left ofthe sidebar/browser content window).
  - Possible solution to look into: delay on `:not:hover` and return the `z-index` to a lower number? That way the animation can complete when not hovered and it can return to a lower z-index.
