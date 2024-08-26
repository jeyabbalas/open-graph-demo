# Open Graph protocol demo

This repository is a test to explore how [Open Graph protocol](https://ogp.me/) works. Note that while Facebook designed this protocol, it also works on other social networking websites. I only tested this on LinkedIn.

The Open Graph protocol enables website developers to embed their websites as feature-rich objects within Facebook's [social graph](https://en.wikipedia.org/wiki/Social_graph), when a user shares their website on Facebook. These objects then become nodes in Facebook's social graph, similar to Facebook users, posts, photos, events, and pages. The Facebook [Graph API](https://developers.facebook.com/docs/graph-api/) is then able to register and query user interactions with the website object along with other objects in the social graph.

The initial version of this protocol is based on [RDFa](https://en.wikipedia.org/wiki/RDFa). To turn their websites into open graph objects, web developers need to at least add 4 basic Open Graph metadata elements to their web page. Using RDFa, web developers must add additional `<meta>` tags to the `<head>` of their web page. The required properties are as follows.
1. `og:title`: The title of your object as it should appear within the graph.
2. `og:type`: The type of your object, e.g., "website", "music.song", "video.movie", "article", etc.
3. `og:image`: An image URL which represents your object within the graph.
4. `og:url`: A canonical URL of the object what will be used as a permanent ID in the graph. 
