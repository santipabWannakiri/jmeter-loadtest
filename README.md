# jmeter-loadtest

### Jmeter load distribution control
- Creating multiple Thread Groups
- Throughput Controller ( Single Thread Groups )

### Load Distribution Comparison

| **Aspect**                  | **Multiple Thread Groups**                                           | **Single Thread Group with Throughput Controllers**              |
|-----------------------------|-----------------------------------------------------------------------|-------------------------------------------------------------------|
| **Technical Term**          | Load Distribution, Request Distribution                              | Load Distribution, Throughput Control                            |
| **Control Over Users**      | High: Separate configuration for each Thread Group (e.g., users, ramp-up, loops) | Medium: Unified user control, percentages managed by Throughput Controllers |
| **Ease of Setup**           | Complex: Requires configuration for each Thread Group separately     | Simple: Single Thread Group setup with percentage-based distribution |
| **Resource Usage**          | Higher: More resource consumption due to multiple Thread Groups       | Lower: More efficient with a single Thread Group                  |
| **Flexibility**             | High: Different behaviors and configurations per Thread Group         | Medium: Less flexibility for individual thread behavior            |
| **Scalability**             | Can become cumbersome with many Thread Groups                        | Scales well with one Thread Group                                  |
| **Test Management**         | More complex: Manage multiple Thread Groups                          | Easier: Manage and adjust within one Thread Group                 |
| **Test Analysis**           | Easier to analyze separately: Results for each Thread Group are distinct | Requires filtering: Results are combined, need to distinguish by request |
| **Best For**                | Complex tests with varied load profiles, different user behaviors    | Simple load distribution, resource-efficient testing               |

#### Key Terms

- **Load Distribution**: The process of allocating a certain percentage of total requests to different APIs or components.
- **Request Distribution**: Refers specifically to the allocation of requests among different API endpoints.
- **Throughput Control**: In JMeter, the Throughput Controller manages how frequently different requests are executed based on specified percentages.
