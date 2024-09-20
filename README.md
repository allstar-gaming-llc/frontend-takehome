# Front-end Takehome Exam

We want to create a simple clip feed with data queried from our GraphQL API.

### Instructions:

1. Set up a basic React app with Typescript. We suggest using [Vite](https://vitejs.dev)
1. Build a video feed that displays clips via data from the `clips` query.
1. Use CSS to style the project how you see fit. This is a front-end test so things like eye for detail, design choices, and style will be taken into account!
1. Push your project to GitHub as a private repository and add collaborators `@bryanmytko` and `@rosscooperman`
1. The project should run locally with no issues or additional requirements.

### Basic requirements:

- Display relevant information such as username, avatar, etc.,
- Video clips should be playable
- The feed should contain at least 3 clips.
- Implement appropriate types/interfaces.
- Write clean code and use best practices!

### Provided information:

**GraphQL Endpoint:** `https://api.prod.allstar.dev/graphql`

**CDN:** `https://stagingmedia.allstar.gg`

Basic clips query looks like:
```
clips(search: $search, limit: $limit, game: $game) {
    data {
        _id
        clipImageThumb
        clipLink
        clipPreviewPath
        clipTitle
        user {
            avatar
            username
        }
    }
}
```

### Important:

1. Use the string `popular` for the search field.
1. For the game field, use either `7302` for Counter-Strike 2 or `101` for League of Legends.
1. Feel free to introspect the graph to find more available fields to make your project stand out!
