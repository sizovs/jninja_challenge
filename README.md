# Homework

### Goal
Create a simple link shortening and analytics web service similar to `bit.ly`.

In order to take over the world and beat competitors, we need the service that provides the following functionality:

### 1) Ability to shorten the link
- Include validation against malformed links

### 2) Ability to customise the link `(bit.ly/<this-part>)`
- Make sure there are no duplicates
- Make sure that `<this-part>` does not include abusive words (provide hard-coded dictionary with `N` random words)

### 3) Ability to track link visits (time, ip address and country).
- Country is resolved against some geo-encoding service such as `ip-api.com` or `freegeoip.net`
- Implement protection against network latency with Hystrix
- Make sure that a link is eventually geo-encoded, even if geo-encoding service is slow or unresponsive during the link visit

### 4) Ability to get all shortened links via web api

### 5) Ability to get all visits for a given link via web api
- It must be clear from the response whether geo-encoding is pending
- Link visits must appear in chronological order

### Other concerns
- Demonstrate application usage with high-level acceptance tests
- Make sure that both application and tests run in embedded mode. In other words, it must run on a laptop with nothing but Java and Docker installed
- Push application to GitHub
- Provide simple and concise setup instructions
- Express major design decisions you have made on wiki

### FAQ
– there is no need in UI. Web API is the app's UI.
