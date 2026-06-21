# Vertical Scaling

- Scaling a server by ram, storage and cpu cores
- Server A - 4CPU 8GB ram upgraded to 16CPU 64GB RAM

## Advantages

- Easy to implement
- No app changes needed
- No load balancer needed

## Disadvantages

- Hardware limits
- Expensive at higher sizes
- Single point of failure - one server down = system down
- Downtime required during upgrades

# Horizontal Scaling

- Adding more machines instead of upgrading single machine

## Example

- Before - Users -> App server
- After - User -> Load Balancer -> App1, App2, App3

## Advantages

- Better fault tolerance
- No upper limit (scale as much as you need)
- High availability
- Supports massive traffic growth

## Disadvantages

- More complex architecture
- Load balancing required
- Distributed system challenges
- Session management becomes harder (req 1 goes to App1, req 2 goes to App2, unless managed using JWT, Redis Session store)

- Horizontal scaling requires
  - Replication
  - Sharding (Sharding is a database architecture pattern that splits a massive dataset into smaller, manageable chunks called "shards")
  - Distributed transactions
  - Consistency handling

## When to use which

- Start with vertical scaling
  - Starting phase of app with 10k daily users
  - Internal apps
  - MVPs

- Move to horizontal scaling when
  - Traffic grows significantly
  - High availability required
  - Single server becomes bottleneck
