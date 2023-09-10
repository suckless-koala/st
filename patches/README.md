## Applying the dracula theme
If using just [st-scrollback-ringbuffer-0.8.5.diff](https://st.suckless.org/patches/scrollback/st-scrollback-ringbuffer-0.8.5.diff), apply `st-dracula-scrollback-ringbuffer-0.8.5.diff`.

If using both [st-scrollback-ringbuffer-0.8.5.diff](https://st.suckless.org/patches/scrollback/st-scrollback-ringbuffer-0.8.5.diff) and [st-focus-20230610-68d1ad9.diff](https://st.suckless.org/patches/alpha_focus_highlight/st-focus-20230610-68d1ad9.diff), apply `st-dracula-focus-scrollback-ringbuffer-0.8.5.diff`.

I have not made a patch for dracula without scrollback-ringbuffer but you can easily copy the colour codes from my config.

## Using both scrollback-ringbuffer and externalpipe
`externalpipe` introduces some new code which relies on code that was modified by `scrollback-ringbuffer`.
My `externalpipe-scrollback-ringbuffer` patch fixes the two guilty lines, allowing both patches to work together.
Make sure to apply both `externalpipe` and `scrollback-ringbuffer` before applying `externalpipe-scrollback-ringbuffer`.

## koala-config
This simply modifies some of st's configuration to suit my preferences more. Note that it assumes that `font2` and `externalpipe`  have been applied.
