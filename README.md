# Shopify Shipping Progress Bar

This repository contains the code for a customizable Shipping Progress Bar for Shopify stores. The Progress Bar displays the progress towards free shipping and motivates customers to add more items to their cart to reach the free shipping threshold.

## Preview

### Goal Not Yet Reached
![Shipping Progress Bar - Goal Not Reached](https://i.postimg.cc/6pwmxTf1/image.png)

*The progress bar shows the current status towards achieving free shipping.*

### Goal Reached
![Shipping Progress Bar - Goal Reached](https://i.postimg.cc/tgg1ftZR/image.png)

*When the goal is reached, free shipping is clearly displayed.*

## Features

- Dynamic progress bar
- Display of current cart value
- Display of remaining amount to free shipping
- Clear indication when free shipping is achieved
- Responsive design
- Customizable colors and text

## Installation

Follow these steps to integrate the Shipping Progress Bar into your Shopify theme:

1. **Open the Theme Code Editor:**
   * In your Shopify Admin, go to `Online Store` > `Themes`.
   * Click on `Actions` > `Edit code` to open the Theme Code Editor.

2. **Find the Correct File:**
   * In the Theme Code Editor, look for the `Snippets` folder.
   * Open the relevant snippet file, typically named `cart-drawer.liquid` or something similar.

3. **Insert the Code:**
   * Search for `</cart-drawer-items>` in the file using `Ctrl + F`.
   * Insert the provided code snippet directly **below** the `</cart-drawer-items>` line and **above** the `<div class="drawer__footer">` line.

   ```liquid
   </cart-drawer-items>
   <!-- Insert the Shipping Progress Bar code here -->
   <div class="drawer__footer">
   ```

4. **Adjust the Variables:**
   * Modify the `free_shipping_threshold` and `shipping_cost` variables at the beginning of the code to match your Shopify store settings.

5. **Save the Changes:**
   * Click `Save` to apply the changes.

## Customization

You can customize the appearance of the Shipping Progress Bar by modifying the following variables in the code:

- `progress_bar_color`: The color of the progress bar
- `background_color`: The background color of the container
- `text_color`: The main text color
- `secondary_text_color`: The color for secondary texts
- `success_color`: The color for success messages

You can also adjust the texts in the HTML part of the code to match your brand's voice.

## Contributing

Contributions are welcome! For major changes, please open an issue first to discuss what you would like to change.

## License

[MIT](https://choosealicense.com/licenses/mit/)
