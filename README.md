This repo present a minimal example of a bug in [lens.vim](https://github.com/camspiers/lens.vim).

## Reproduction steps

Install plugins mentioned in `init.vim`.

1. Run `nvim -u init.vim example.txt`
2. Call FZF: `:FZF`
3. Select a file and press `C-v` to open it in a vertical split.

You'll see that lens.vim stretches the opened window to the maximal allowed
width.

The expected behaviour is for lens.vim to open the new window with equal width.

## Video

`screencast.mp4` presents the bug.
