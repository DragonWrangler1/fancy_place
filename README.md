# Fancy Place Mod

A simple block placement system for Minetest that allows placing block B next to block A without pointing at block A.

## Features

### 🎯 Simple Horizontal Placement

1. **Horizontal-Only Placement**
   - Blocks can only be placed next to other blocks on the same Y level (horizontally)
   - Supports both cardinal directions (north, south, east, west) and diagonal directions
   - No special placement on top of blocks or below blocks
   - Prevents accidental vertical stacking

2. **Smart Adjacent Detection**
   - When aiming at air, automatically finds nearby horizontal surfaces to place against
   - Checks 8 horizontal directions: 4 cardinal + 4 diagonal
   - Searches within reach distance (4.5 blocks, but configurable)
   - Should work with all standard Minetest blocks

3. **Cross-Platform Input Support**
   - **Desktop/PC**: Uses right-click to place blocks
   - **Android/Touch Devices**: Automatically detects touch controls and uses tap (punch) to place blocks
   - Seamless experience across all platforms without manual configuration

## Installation

1. Download or clone this mod to your Minetest mods directory
2. Enable the mod in your world settings
3. Start playing with block placement!

## Usage

### Basic Usage
- Hold any placeable block in your hand
- Look around - you'll see semi-transparent ghost blocks appear next to existing blocks (horizontally only)
- **Desktop/PC**: Right-click on a ghost block to place the real block there
- **Android/Touch Devices**: Tap (punch) on a ghost block to place the real block there
- The block will be consumed from your inventory (unless in creative mode)
- No configuration needed - it just works!

### How It Works
- When you hold a placeable block, the mod shows a semi-transparent ghost block at valid horizontal placement positions
- Ghost blocks only appear next to other blocks horizontally (same Y level) - never on top or below
- **Desktop/PC**: Right-click the ghost block to place the actual block and consume it from your inventory
- **Android/Touch Devices**: Tap (punch) the ghost block to place the actual block and consume it from your inventory
- The mod automatically detects if you're using touch controls and adjusts the input method accordingly
- Normal block placement is not overridden - this only adds the ghost block preview system

## Compatibility

- Should work with all standard Minetest nodes
- Compatible with most other mods
- Maintains all original node placement callbacks and behaviors

## Technical Details

- Minimal performance impact with simple algorithms
- Fallback to original placement behavior when horizontal placement fails
- No configuration files or settings needed

## Contributing

Feel free to submit issues, suggestions, or pull requests to improve the mod!

## License

See `license.txt` for licensing information.
