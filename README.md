# philippine-holidays-json
basic json file for holidays. feel free to update.

# usage: easy api no need web scraping

# ex js:

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



