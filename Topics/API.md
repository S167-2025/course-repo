# JSON and API

### JSON
JavaScript Object Notation (JSON) is a string whose format very much resembles JavaScript object literal format. The following is a valid JSON string representing an object.

Exercise: write a JSON file together

### API
An application programming interface (API) is a connection between computers or between computer programs. It is a type of software interface, offering a service to other pieces of software. A document or standard that describes how to build such a connection or interface is called an API specification. A computer system that meets this standard is said to implement or expose an API. The term API may refer either to the specification or to the implementation.

In real life, software API usually means a set of data that is accessible from a server. Access the following URL and see the data from our Reading Response Are.Na channel:
```
https://api.are.na/v2/channels/reading-responses-g2pohw2w5jk?per=100
```

We can use the `fetch` function to send an HTTP request to get data from an API into our application:
```
async function getArenaData() {
const channel = 'eggs';
const url = `https://api.are.na/v2/channels/${channel}?per=100`;
  
try {
  const response = await fetch(url, { cache: 'no-store' });
    
  if (!response.ok) {
    throw new Error(`Response status: ${response.status}`);
  }

  const data = await response.json();
    
  // Log the full data object
  console.log('Full channel data:', data);
    
  // Log specific parts you might be interested in
  console.log('Channel title:', data.title);
  console.log('Channel description:', data.metadata?.description);
  console.log('Contents:', data.contents);
  console.log('Number of items:', data.contents?.length);
    
  } catch (error) {
    console.error('Error fetching Are.na data:', error.message);
  }
}

// Call the function
getArenaData();
```

Download and work with the Are.Na API [demo file](/_assets/arena-api.zip) for project *Legend*, creating a digital publication platform.
