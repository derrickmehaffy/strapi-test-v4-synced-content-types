# Synced content-types example

**NOTE: You will not be able to use the content-type builder on any content-types using this method, if you do it will move them out of sync**

What has been done:

- Converted each content-type's `schema.json` to a `schema.js` file
- Created a central content-type storage location
- Import the central content-type and set the values (you can't just mirror the whole schema file as there is content-type independent settings)

Content-types:

- [Company 1 Blog Posts](src/api/company-1-blog-post/content-types/company-1-blog-post/schema.js)
- [Company 2 Blog Posts](src/api/company-1-blog-post/controllers/company-1-blog-post.js)
- [Central Blog Post content-type attributes](src/synced-content-types/blog-post/attributes.json)
- [Central Blog Post content-type options](src/synced-content-types/blog-post/options.json)

## Instructions to add new attributes

Edit the synced content-type's attribute file manually to modify both content-types. As mentioned in the note above it is not possible to use the content-type builder on content-types that are considered "synced".
