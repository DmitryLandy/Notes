# Scalability
## Sharding
- Distributing data across multiple horizontally scaled instances.
- 

## Normalize vs De-Normalize
Normalized: less storage and easier to update, but requires more lookups. SQL
Denormalized: More storage, one lookup, difficult updates

**Scenario:**
Reservations require customer id, which requires customer table (2 tables total). Normalized would have to query both tables. Denormalized would only have 1 table but duplicate data in table.

## Big Data / Distributed Storage
Data lakes such as S3 or blob storage can be used for general storage and then use Redshift or Synapse to process it

## ACID
A: Atomic (Query fully succeed or fails)
C: Consistent (All rules are enforced or transaction is rolled back)
I: Isolated (queries are independent when being run, and can't be altered while in progress)
D: Durability ( If transaction is completed, it stays even after immediate server crash)

## CAP Theorem
3 parts: Consistency, Availability, Partition-Tolerence
Must comromize on one part 

EXAMPLES

![[Pasted image 20220521122450.png]]

## SLA
Ask what the accepted SLA is for the service.

## Message Queues
Helps decouple prducer/consumer requests. Helps managed backed up requests so they don't get dropped

Used as a buffer

## Apache Spark
- Process large amounts of data
- Can be real time, graph processing, pattern mining (ML algorithms)

