# How is this website composed?

#### 'Just like each family member contributes to becoming an Eternal Family, each code serves a purpose to make this blog/article website work' -Doss

### Vue 3.2 and the Composition API

Vue 3.2 introduces several improvements and new features, including the Composition API, which provides a more flexible and organized way to structure Vue components. Instead of the traditional options API, where the component's logic is divided by options (methods, computed properties, data, etc.), the Composition API allows developers to group logic by feature. This is particularly useful in a blog page where you might have functionalities such as fetching posts, parsing markdown content, and handling user interactions.

For 'Why Have an Eternal Family?' Blog Page, the Composition API facilitates the creation of composable functions for different aspects of the blog, such as fetching blog posts from a static file or an external API, handling markdown parsing, and managing user comments or reactions if included. These composables can then be reused across different parts of the application, promoting code reuse and maintainability.

### Pinia for State Management

Pinia is the officially recommended state management library for Vue.js. It is designed to be more intuitive and easier to use than its predecessor, Vuex. In the context of 'Why Have an Eternal Family?' Blog Page, Pinia would be responsible for managing the state of the blog, such as the list of blog posts, the current post being viewed, and potentially user settings if the blog supports customization features.

Pinia stores could be used to fetch and cache blog posts, making them readily accessible throughout the user's session. This approach simplifies state management and ensures that the application remains responsive and efficient.
Vite for Project Building

Vite is a modern build tool that leverages ES modules to serve code via HTTP in development, allowing for lightning-fast hot module replacement (HMR). For production, it bundles the application using Rollup, ensuring optimal performance. In 'Why Have an Eternal Family?' Blog Page, Vite would streamline both development and production builds, ensuring that the blog loads quickly and efficiently, providing a smooth user experience.

### Axios for HTTP Requests

Axios is a promise-based HTTP client that simplifies making HTTP requests to fetch or save data. For a blog like 'Why Have an Eternal Family?' Blog Page that does not use a database but might fetch blog posts from a static file or an external API, Axios is ideal for handling these requests. It can be used to asynchronously fetch the blog posts' data and handle any HTTP interactions the blog might require, such as posting comments or fetching external resources.

### Bulma for Styling

Bulma is a modern CSS framework based on Flexbox, providing a comprehensive set of responsive and mobile-first components. In 'Why Have an Eternal Family?' Blog Page, Bulma can be used to style the blog's interface, ensuring that the blog is visually appealing and accessible across all devices. The use of Bulma facilitates rapid UI development, allowing more focus on the blog's functionality rather than the intricacies of CSS.

### Marked for Markdown Parsing

Marked is a markdown parser and compiler. Given that 'Why Have an Eternal Family?' Blog Page might store blog posts in markdown for simplicity and ease of editing, Marked would be instrumental in converting markdown content into HTML that can be rendered on the blog page. This allows for a seamless workflow where blog posts can be written, previewed, and published in markdown, simplifying content creation.

### Putting It All Together

Combining these technologies, the Blog page of 'Why Have an Eternal Family?' Blog Page would likely involve a Vue component utilizing the Composition API to manage the lifecycle and logic of the blog page. Pinia stores would manage the state, such as the current posts and any user settings or preferences. Axios would fetch blog post data, which would then be parsed by Marked and styled using Bulma for presentation. Vite ensures that the development experience is smooth and that the final build is optimized for performance.

The Composition API functions would be responsible for fetching and displaying posts, parsing markdown content, and any other interactive elements on the page. Pinia's integration ensures that the blog's state is centrally managed and easily accessible, making the application scalable and maintainable. Together, these technologies enable the creation of a fast, responsive, and user-friendly blog platform, fulfilling the aims of 'Why Have an Eternal Family?' Blog Page to leverage the latest in Vue development without the complexity of database management.