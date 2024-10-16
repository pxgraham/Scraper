Uses `express` for the server, `mongoose` for MongoDB interaction, `axios` for HTTP requests, and `cheerio` for HTML parsing.

`axios` fetches HTML from the EchoJS website.
`cheerio` parses the HTML and selects all `<h2>` elements within `<article>` tags.

A GET route at `/articles` fetches all articles from the database and returns them as JSON.

A GET route at `/articles/:id` fetches a specific article by its ID and populates its associated notes.

A POST route at `/articles/:id` creates a new note and associates it with an article by updating the article’s note field.