# Instructions
* In console: open index.html
* In file: click on index.html
* Start using app by allowing location service  
* The entire application is accomplished in vanilla javascript, if you want to see this application implemented in other frameworks, I can also do it in React. 

# Current location
* app will ask for current location to show nearby places
* current location is displayed on the nav bar 

# Inputs 
## Category
   * Categories are provided by google places, all types are queried from the document, see bottom of the page to see how I did it
   * Choosing a category will re-render the map and list with places related to that type 

## Search Input 
   * Text input will re-render map and list with places related to the key word 

# Markers 
* onClick will pop up a small infoWindow with location name 
* onClick will also recenter the map for better viewing 

# List
* onClick will select the relevant marker and trigger it's infoWindow eventListener for info and recenter 

# Grab all location types from google document 
https://developers.google.com/places/supported_types
  ```javascript
  const array = Array.from(document.querySelectorAll('.column ul li code'));
  array.map(el => el.innerHTML);
  ```

