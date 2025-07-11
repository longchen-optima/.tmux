# tmux Configuration Upgrade Notes

This update enhances the tmux configuration to take advantage of features available in tmux 3.5 and newer versions.

## Key Improvements

1. **Performance Optimizations**
   - Reduced escape-time to 10ms (default in tmux 3.5+)
   - Added prefix timeout option for better key handling

2. **Extended Key Support**
   - Enabled extended keys support with mode 2 format
   - Improved handling of modifier keys

3. **New Layout Options**
   - Added mirrored versions of main-horizontal and main-vertical layouts
   - Added key bindings for these new layouts (M-v and M-h)

4. **Enhanced Visual Features**
   - Added popup window styling with rounded borders
   - Added underscore color support for pane borders
   - Added search count display in status line

5. **Hyperlink Support**
   - Enabled OSC 8 hyperlink support for terminal links

6. **Error Handling**
   - Added command error hook for better debugging

7. **Recommended Plugins**
   - Added tmux-resurrect and tmux-continuum for session persistence
   - Added tmux-yank for improved clipboard integration

## Usage

To use this updated configuration:

1. Replace your existing `.tmux.conf.local` with the updated version
2. Reload tmux configuration with `tmux source-file ~/.tmux.conf`

## Requirements

- tmux version 3.3a or newer (recommended: 3.5+)
- For full feature support, a terminal that supports:
  - 24-bit color
  - Extended keys
  - Hyperlinks (for OSC 8 hyperlink support)

## Compatibility

This configuration maintains backward compatibility with older tmux versions while enabling new features when available.