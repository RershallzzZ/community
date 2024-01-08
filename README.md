# community
A community forum for programmers that supports basic functions such as registration, login, profile setting, direct message, post, comment, like and follow modules with efficient file storage in AWS S3.
- Utilized Redis HyperLogLog to estimate the count of unique visitors (UV) and Bitmaps to track the Daily Active User (DAU).
- Implemented role-based access control with Spring Security and used Elasticsearch for global search functionality, incorporating keyword highlighting to enhance user search experience.
- Developed a hot posts ranking feature using a multi-level caching strategy with Caffeine as the local cache and Redis for distributed cache, preventing cache avalanche issues and improving the website’s query performance by 19.7 times (from 9.5 QPS to 186.8 QPS).
- Integrated Kafka to manage system notifications for comments, likes, follows, and asynchronously relay new posts to the Elasticsearch server, encapsulating these processes within events for a robust message system.
