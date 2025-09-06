# CashCats13K - Cat Collector Game

A fun idle/clicker game where you manage cats that collect coins and need care. Built for the js13k game jam.

## Game Features

### Core Gameplay
- **13 Cats**: Each with unique names and behaviors
- **Coin Collection**: Cats automatically collect coins scattered around the game area
- **Cat Care System**: 
  - Feed cats with fish 🐟 to fully satisfy love 💖
  - Pet cats 💖 to increase love and speed
  - Cats need water 💧 when thirsty
- **Upgrade System**: Improve cat speed and carrying capacity
- **Special Cat**: Kitty13k with constant upgrade costs and enhanced stats

### Cat Management
- **Hunger System**: Cats get hungry and need fish
- **Thirst System**: Cats need water to stay hydrated  
- **Love System**: Petting cats increases their love and speed
- **Sad State**: Cats become immobilized when love is too low
- **Carrying Capacity**: Cats can carry multiple coins before returning to base

### Responsive Design
- **Mobile Optimized**: Touch-friendly controls and responsive layout
- **Multiple Breakpoints**: Adapts to different screen sizes
- **Landscape Support**: Special layout for mobile landscape mode
- **5-Column Layout**: Upgrade panel displays cats in 5 columns (1-3-3-3-3 distribution)

## File Structure

- `CashCats13K.html` - Last Version for js13k submission
- `README.md` - This documentation file

## Technical Details

### Technologies Used
- **HTML5**: Semantic structure
- **CSS3**: Responsive design with Grid and Flexbox
- **Vanilla JavaScript**: No external dependencies
- **Touch Events**: Mobile-friendly interaction

### Key Features
- **No localStorage.clear()**: Compliant with js13k rules
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Touch Controls**: Drag and drop fish feeding on mobile
- **Performance Optimized**: Efficient game loop with requestAnimationFrame

### Cat Distribution
- **Column 1**: Kitty13k (special cat)
- **Column 2**: Whiskers, Mittens, Paws (3 cats)
- **Column 3**: Luna, Shadow, Bella (3 cats)  
- **Column 4**: Max, Lily, Tiger (3 cats)
- **Column 5**: Milo, Nala, Oreo (3 cats)

### Special Cat - Kitty13k
- **Base Speed**: 180px/s (vs 65px/s for others)
- **Carrying Capacity**: 18 coins (vs 6 for others)
- **Upgrade Costs**: Always 13g (doesn't increase)
- **Position**: First column, highlighted as special
- **No Hunger**: Doesn't have hunger bar or get hungry
- **Special Sad Behavior**: When love is low, continues moving randomly but doesn't collect coins
- **Recovery**: Only returns to normal when love bar is completely filled by clicking

## Controls

### Desktop
- **Click cats**: Pet them to increase love
- **Drag fish**: Click and drag fish to give full love to cats
- **Click coins**: Collect coins manually
- **Upgrade buttons**: Click to upgrade cat stats

### Mobile
- **Touch cats**: Pet them to increase love
- **Drag fish**: Touch and drag fish to feed cats
- **Touch coins**: Collect coins manually
- **Upgrade buttons**: Touch to upgrade cat stats

## Game Mechanics

### Cat States
1. **Idle**: Normal state, collecting coins
2. **Hungry**: Needs fish, shows 🐟 above cat
3. **Thirsty**: Needs water, shows 💧 above cat
4. **Sad**: Low love, shows 💖 above cat, immobilized
5. **Drink**: Drinking water at water source

### Resource Management
- **Gold**: Earned by cats returning coins to base
- **Fish**: Drag to give full 💖 to cats
- **Water**: Cats automatically go to water source when thirsty
- **Love**: Increased by petting, affects cat speed

### Upgrade System
- **Speed Upgrade**: +15px/s speed increase
- **Capacity Upgrade**: +4 coin carrying capacity
- **Cost Scaling**: Costs increase by 13g per upgrade (except Kitty13k)
- **Special Pricing**: Kitty13k maintains constant 13g cost

## Development

### Code Structure
- **Modular Design**: Separate functions for different game systems
- **Object-Oriented**: Cat class with methods for behavior
- **Event-Driven**: Responsive to user interactions
- **Performance Focused**: Optimized rendering and updates

### Responsive Breakpoints
- **Desktop**: >1000px - Full layout
- **Tablet**: 600-1000px - Adjusted sizing
- **Mobile Portrait**: <600px - Stacked layout
- **Mobile Landscape**: <600px landscape - Compact layout
- **Small Mobile**: <480px - Minimal layout

## Browser Compatibility

- **Modern Browsers**: Chrome, Firefox, Safari, Edge
- **Mobile Browsers**: iOS Safari, Chrome Mobile, Samsung Internet
- **Touch Support**: Full touch event handling
- **Responsive**: Adapts to any screen size

## Performance

- **60 FPS**: Smooth animation with requestAnimationFrame
- **Efficient Rendering**: Minimal DOM manipulation
- **Memory Management**: Proper cleanup of event listeners
- **Touch Optimization**: Responsive touch controls

## License

Created for js13k 2024. All rights reserved.

## Credits

- **Game Design**: Original concept and implementation
- **Art Assets**: Emoji-based graphics
- **Code**: Vanilla JavaScript implementation
- **Responsive Design**: Mobile-first approach
