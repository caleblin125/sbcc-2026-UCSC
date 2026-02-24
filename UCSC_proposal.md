# Not So Slow Slugs

Team Logo here
<!--
<img src="" alt="" height="200"/>
-->

## Diagram


## Hardware

We originally expected to recieve \$6k in funding instead of having a \$6k budget cap. Because of this, we had to scale back our original plans and use more of what we already had. Our Faculty advisor has a 10 RPi5-node picocluster worth $3k that we are using. This will be great for general worker nodes but we still needed some specialized boards for acceleration of the tasks. MDTest is dependent more on I/O speed which doesn't benefit from the compute capabilities of the 10 RPis. The raspberry Pis only expose a single lane of PCIe 2.0, which is quite slow compared to today's standards. To solve this, we needed something wth at least PCIe Gen3 x4. Thankfully, the Jetson Orins have this, so they can double as the GPU nodes and the fast storage nodes. Additionally, we may acquire 1 or 2 LattePanda IOTA though sponsorships, which will be supporting our CPU compute.

### Power monitoring
Describe your plan to report your system's power draw to the committee. In the past we have had Grafana displays or livestreamed footage of the power reading; we will work with you to confirm the details of this plan. 

### Hardware Table 

Example: 

250W Total

| Item | Amount | Purpose | Expected Power Draw | Price|
| -------- | ------- |------- |------- |------- |
| Raspberry Pi 5  | 10 | CPU Compute | 120W (12W) | $3000 |
| Jetson Orin Nano | 2 | GPU Compute | 50W (25W) | $300 |
| LattePanda Iota (Intel N150, 8GB RAM / 64GB eMMC) | 2  | CPU Compute| 48W (24W) | $260 |
| NETGEAR 24-Port Gigabit Ethernet Unmanaged Switch (JGS524) | 1     | | | |

## Software

We will be using ubuntu on all our devices due to it's familiarity and support. On top of that we will use Slurm scheduler to run the benchmarks on our cluster. 

## Strategy

### Benchmarks

Explain your initial strategy for completing the benchmarks. 

### Applications

Explain your initial strategy for completing the applications. 

## Team Details

List your team members and a brief description of interests and skills.
