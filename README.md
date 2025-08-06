# Philippine Holidays JSON

This repository contains a simple JSON list of official Philippine holidays.

You can access the raw JSON file directly via:

https://raw.githubusercontent.com/estelsnt/philippine-holidays-json/main/holidays.json


## How to Fetch in Browser

Here's a basic example of how to fetch and use the data in plain JavaScript (browser):

```html
<script>
  fetch('https://raw.githubusercontent.com/estelsnt/philippine-holidays-json/main/holidays.json')
    .then(response => {
      if (!response.ok) {
        throw new Error(`HTTP error! status: ${response.status}`);
      }
      return response.json();
    })
    .then(data => {
      console.log('📅 Philippine Holidays:', data);
    })
    .catch(error => {
      console.error('Error fetching holiday data:', error);
    });
</script>
