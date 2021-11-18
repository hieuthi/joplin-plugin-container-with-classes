# Container with Classes

Plugin for creating block-level containers with classes for Joplin notes, it is based on [markdown-it-container](https://github.com/markdown-it/markdown-it-container) with some changes.

```
::: classname1 classname2 classname3
**Bold Text**
:::
```

which will be rendered as follow:
```
<div class="classname1 classname2 classname3">
  <strong>Bold Text</strong>
</div>
```

For nested div the parent need to have more ":" than chils:
```
:::::: parentclass

Parent text

::: childclass
**Bold Text**
:::

::::::
```

**Why do you want to use this plugin instead of directly write html tag?**
Because, you can't write markdown syntax within html. Using this plugin markdown text will be rendered as usual.

![Examples](https://github.com/hieuthi/joplin-plugin-container-with-classes/docs/preview.png)

There is no pre-defined class, you have to define them within the note or in `userstyle.css` yourself. 
You can copy the content of [examples.md](https://github.com/hieuthi/joplin-plugin-container-with-classes/docs/examples.md) to joplin to see some simple examples. It includes:

- Multi-column Paragraph
- Center-Aligned Paragraph
- Always-On Drawer
- Vertical Right-to-Left Paragraph
- Custom Container

## License
[MIT](https://github.com/hieuthi/joplin-plugin-container-with-classes/LICENSE)