# CAP Theorem (Brewer's Theorem)

> "In a distributed data store, you can only provide two of the following three guarantees: Consistency, Availability, and Partition Tolerance."

**The Insight:**

- **Consistency:** Every read receives the most recent write or an error.
- **Availability:** Every request receives a (non-error) response, without the guarantee that it contains the most recent write.
- **Partition Tolerance:** The system continues to operate despite an arbitrary number of messages being dropped/delayed by the network.
  Since networks _do_ fail (Partition Tolerance is a reality), you must choose between Consistency (CP) and Availability (AP) during a failure.

**In Practice:**  
Stop looking for a "perfect" database. Decide what your business can tolerate. Is it okay if a user sees an old like count for a few seconds (AP)? Or is it critical that a bank transfer is atomic even if the system has to go down to ensure it (CP)?
