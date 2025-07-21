# Fancy Place Mod - User Guide

## What does this mod do?

The Fancy Place mod makes building easier by showing "ghost blocks" - transparent preview blocks that appear next to existing blocks. You can right-click these ghost blocks to place your blocks exactly where you want them!

## Key Features

- 🔍 **Ghost Block Preview**: See exactly where your block will be placed
- 🎯 **Horizontal Placement Only**: Only places blocks next to other blocks (not on top or below)
- ⚙️ **Fully Customizable**: Easy-to-use configuration file
- 🎨 **Visual Feedback**: Transparent, glowing preview blocks
- 🔒 **Protection Aware**: Respects area protection mods

## How to Use

1. **Hold a block** in your hand (any placeable block)
2. **Look near existing blocks** - you'll see transparent "ghost blocks" appear
3. **Right-click a ghost block** to place your block there
4. **That's it!** The block is placed and the ghost block disappears

## Customizing the Mod

### Easy Way (Recommended)
1. **In-Game Settings Menu**:
   - Go to Settings → All Settings
   - Navigate to Mods → fancy_place
   - Adjust the settings with sliders and checkboxes
   - Changes take effect immediately!

2. **Configuration File Method**:
   - Add settings to your `minetest.conf` file
   - Restart your world for changes to take effect

### Available Settings
```
fancy_place_ghost_opacity = 128        # Ghost transparency (0-255)
fancy_place_ghost_glow = 8             # Ghost glow intensity (0-15)  
fancy_place_ghost_size = 1.02          # Ghost size multiplier (1.0-1.1)
fancy_place_reach_distance = 4.5       # How far you can place (1.0-4.5)
fancy_place_allow_diagonal = true      # Allow diagonal placement
fancy_place_play_sounds = true         # Play placement sounds
fancy_place_update_interval = 0.2      # Update frequency in seconds
fancy_place_instant_updates = true     # Instant ghost block updates
fancy_place_show_config = false        # Show config in server log
```

## Configuration Options

### Ghost Block Appearance
- **Opacity**: How transparent the ghost blocks are (0-255)
- **Glow**: How much the ghost blocks glow (0-15)
- **Size**: How much bigger ghost blocks appear than normal blocks

### Placement Behavior
- **Reach Distance**: How far you can place blocks
- **Diagonal Placement**: Whether to show ghost blocks diagonally
- **Placement Sounds**: Whether to play sounds when placing blocks

### Performance Settings
- **Update Interval**: How often ghost blocks update
- **Instant Updates**: Whether ghost blocks update immediately
- **Max Ghost Blocks**: Maximum number of ghost blocks per player

## Quick Setup Presets

The `config.lua` file includes several presets you can uncomment:

- **Subtle**: Barely visible ghost blocks for minimal distraction
- **Obvious**: Very visible ghost blocks for easy spotting
- **Performance**: Optimized settings for slower computers
- **Creative**: Extended reach and enhanced visibility for creative building

## Troubleshooting

### Ghost blocks are too hard to see
- Increase `GHOST_OPACITY` (try 180-200)
- Increase `GHOST_GLOW` (try 12-15)
- Increase `GHOST_SIZE` (try 1.03-1.05)

### Ghost blocks are too distracting
- Decrease `GHOST_OPACITY` (try 80-100)
- Decrease `GHOST_GLOW` (try 3-5)
- Decrease `GHOST_SIZE` (try 1.01)

### Performance issues
- Set `INSTANT_UPDATES = false`
- Increase `UPDATE_INTERVAL` to 0.5
- Decrease `GHOST_GLOW` to 3-5

### Ghost blocks don't appear
- Make sure you're holding a placeable block
- Make sure you're looking near existing solid blocks
- Check that the area isn't protected
- Try increasing `REACH_DISTANCE`

## Tips for Best Experience

1. **Start with defaults** - The default settings work well for most players
2. **Adjust opacity first** - This has the biggest visual impact
3. **Test in creative mode** - Easier to experiment with different blocks
4. **Consider your playstyle** - Builders might want higher opacity, casual players might prefer subtle
5. **Performance matters** - If you have a slower computer, use the Performance preset

## Support

If you encounter issues:
1. Check this guide first
2. Try the default settings
3. Look at the console/log for error messages
4. Report bugs with specific details about what you were doing

Enjoy building with Fancy Place! 🏗️
