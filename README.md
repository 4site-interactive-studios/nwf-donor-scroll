# NWF Donor Scroll

This project adds a simple donor scroll that displays the recent donations. It will display the first name, first letter of the last name, and the donation amount of the donor. It will also replace the name of the donor when they want to be anonymous. The animation will pause when the ticker scrolling has been hovered.

## How to add it to Engaging Networks

1. Upload the `donor-scroll.js` file to Engaging Networks.
2. Add the following code block to your EN Page, where you want the donor scroll to appear:
   ```html
   <div id="donor-ticker" data-layout="normal"></div>
   <script src="{EN_ASSETS_URL}/donor-scroll.js"></script>
   ```
3. Replace `{EN_ASSETS_URL}` with the URL of the uploaded file.
4. Save the page.

**Tip**: On NWF's EN account, there's a Code Block saved in the Library that you can use to add the donor scroll to any page. The Code Block is named **"Donor Scroll Normal Width"**.

## How to customize the donor scroll names

To make the Donor Scroll use a pre-defined list of names, you can add a Text Block to the page with a bullet list of names. The Text Block should have the CSS Class `donor-list`, and can be as big as you want.

This is an example of the Text Block content:

```html
<ul>
  <li>Test Aniko J. donated $103.00</li>
  <li>Test Alaine C. donated $36.05</li>
  <li>Test Crystal C. donated $154.50</li>
  <li>Test Dianne M. donated $51.50</li>
  <li>Test David L. donated $72.10</li>
  <li>Test Stuart S. donated $10.00</li>
  <li>Test John A. donated $154.50</li>
</ul>
```

This is a screenshot of the custom CSS class: https://cln.sh/fRblbfQd

## Development

1. `git clone` this repository
2. `npm install` to install dependencies
3. `npm run build` to build the project
4. `npm run watch` to start the development server

## Customizing the donor scroll

You can change the `data-layout` attribute of the `#donor-ticker` element from `normal` to `full` to make the donor scroll use the full width of the page. When using the `full` layout, the donor scroll will stay fixed at the top of the page when scrolling down.

**Tip**: On NWF's EN account, there's a Code Block saved in the Library that you can use to add the donor scroll to any page. The Code Block is named **"Donor Scroll Full Width"**.
