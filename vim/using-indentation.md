# Using indentation
Via [Upcase - Art of Vim](https://upcase.com/videos/indenting-with-ben-orenstein)

It is possible to use `>` to indent only one line one level, but it is better to use `==` that indent the line to the correct level according with your tab settings.

You can use `=` (single instead of double) with a motion, then you can do like `40=` and indent the next 40 lines.

To indent the entire file you should use `gg=G`. That is `gg` to go to begin of the buffer, `=G` to indent till the end of the buffer.

You can also map it to a key using marks functionality to put the cursor back where it was before indent:

```VimL
<Leader>i mmgg==G`m<CR>`
```

Where: `mm` drop a mark where the cursor is at when the key is pressed. Then indent from the beginning till the end of the buffer. And then use `` `m`` for going back where the mark was dropped.
