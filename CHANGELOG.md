# 0.1.3-dev

- Bug fix: Newlines in diagnostics are replace with '\n' to avoid multiline
  messages

# 0.1.2

- Bug fix: Leave a jump in the jumplist when moving to a definition in the same
  file
- Completion improvements:
  - Overwrite `completeopt` before completion for a better experience.
  - Avoid completion requests while already giving suggestions
  - Improve heuristics for start of completion range
  - Flush file changes after completion
- Bug fix: Don't change window highlights when in select mode
- Bug fix: Location list is cleared when switching to a non-tracked filetype,
  and kept up to date across windows and tabs showing the same buffer

# 0.1.1

- Call initialize first for better protocol compliance
- Use a relative path where possible when jumping to definition
- Only display 'message' field for errors
- Bug Fix: Less likely to delete inserted text when trying to complete
- Bug Fix: More likely to try to complete when not following a '.'
- Populate location list with diagnostics
- Bug fix: Don't try to 'edit' the current file

# 0.1.0

Experimental first release - there are protocol bugs, for instance this does not
call the required `initialize` method. Only known to work with the
`dart_language_server` implementation.

Supports:
- Diagnostic highlights
- Autocomplete suggestions
- Jump to definition