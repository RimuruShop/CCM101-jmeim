**Reflection**

It's worth checking the host server's resources even when the containers are running fine, because every container depends on the host underneath it. A container can be set up perfectly and still fail if the machine hosting it runs low on RAM or disk space. It simply can't outperform the hardware it runs on.

If a user reported that they couldn't log in, I would run `docker logs` to see the exact HTTP requests that reached the server around the time of the complaint. I'd watch for failed authentication attempts, 500-level server errors, or requests that never finished. These would show whether the issue came from the client, the network, or the application itself.

Logs and metrics differ in the kind of answer they give. Logs (Checkpoint 4) are detailed, timestamped records of individual events, so they explain why something happened. Metrics (Checkpoint 5) are numerical readings such as CPU percentage and memory usage, taken over time, so they show what is happening at the moment. In short, monitoring tells you a problem exists, and logs help you investigate its cause.

Large companies running thousands of containers depend on centralized tooling instead of checking each one by hand. Prometheus collects metrics from every server and container at regular intervals and keeps them in a time-series database. Grafana then presents that data as dashboards that engineers can read at a glance. This approach scales to entire fleets of machines, which running `docker stats` on one container at a time never could.

My skill at troubleshooting Linux environments has grown noticeably through this lab. Rather than guessing the cause from symptoms alone, I now turn first to real data. I check resource usage with `free`, `df`, and `top`, then compare it with container logs and live metrics before concluding what is actually wrong.
