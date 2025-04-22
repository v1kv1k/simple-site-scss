# Simple Site - SCSS Refactoring

This project refactors the original CSS of the "Simple Site" template into a modular SCSS structure.

## SCSS Structure

The SCSS code is organized using the 7-1 pattern (though simplified to 4 main folders):

```
scss/
|-- abstracts/           # Variables, mixins, and functions
|   |-- _variables.scss  # Global variables
|   |-- _mixins.scss     # Reusable mixins
|   |-- _index.scss      # Forward all abstracts
|
|-- base/                # Base styles
|   |-- _reset.scss      # Reset and base styles
|   |-- _typography.scss # Typography styles
|   |-- _index.scss      # Forward all base styles
|
|-- components/          # Reusable components
|   |-- _project-icon.scss # Project icon component
|   |-- _index.scss      # Forward all components
|
|-- layout/              # Layout sections
|   |-- _container.scss  # Container styles
|   |-- _first-screen.scss # First screen section
|   |-- _about-me.scss   # About me section
|   |-- _numbers.scss    # Numbers section
|   |-- _video.scss      # Video section
|   |-- _footer.scss     # Footer styles
|   |-- _index.scss      # Forward all layout styles
|
|-- main.scss            # Main file that imports all other files
```

## SCSS Features Used

- **Variables**: Custom variables for colors, fonts, spacing, etc.
- **Nesting**: Selector nesting for better readability
- **Mixins**: Reusable style patterns
- **Media Query Mixins**: Media queries wrapped in mixins
- **@forward and @use**: Modern module system for better organization
- **BEM Methodology**: Using BEM naming convention for classes

## How to Use

1. Install dependencies:
   ```
   npm install
   ```

2. Compile SCSS to CSS:
   ```
   npm run sass
   ```

3. Watch for changes and automatically recompile:
   ```
   npm run sass:watch
   ```

4. Build for production (minified CSS):
   ```
   npm run build
   ```

## Main Features

- **Modular Structure**: Each component and section has its own file
- **Responsive Design**: Responsive layouts for different screen sizes
- **Maintainable Code**: Well-organized and documented code
- **DRY Approach**: Using mixins to prevent code duplication 