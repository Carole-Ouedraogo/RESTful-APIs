# Important Concepts

# Consuming an API is slow.
    We have to implement them carefully because it’s an extra HTTP request performed in the server side, so it can increase considerably the time consumed during the request/response cycle. Caching is fundamental to assure the performance of the application.

# You have no control over the API.

    It’s a third-party API, it may stop working without any notice. Something could change, the API server may go down. So be prepare to handle exception cases.

# APIs are usually limited by number of requests you can make.

    Usually, the API provider only let use do a handful of requests per hour. This limit can vary, but usually it’s there. So, we have to take it into account when implementing the integration. Caching usually is the solution for the rate limits.

# Secure your API keys.

    Some APIs will required authentication, meaning you will have deal with sensitive data. Never commit this kind of information to public repositories.

# There’s probably a Python client for it.

    Using a native Python client to access an API is usually a good idea. It makes the authentication process and the usage of its resources easier. Always check first if there is a Python client available. In some cases there will be even multiple options. In such cases, check their repositories first and pick the one with most active development.


    jinja