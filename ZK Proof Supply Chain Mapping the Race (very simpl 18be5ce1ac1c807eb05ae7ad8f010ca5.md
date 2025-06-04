# ZK Proof Supply Chain: Mapping the Race (very simplified, mostly Delphi Reports, RiskZero’, Taiko, Succinct, EF team tweets and personal questionaries; aaand of course GPT o3-mini high)

Status: No
Status 1: Done

# **Table of Contents**

1. [Executive Summary](https://www.notion.so/ZK-Proof-Supply-Chain-Mapping-the-Race-very-simplified-mostly-Delphi-Reports-RiskZero-Taiko-S-18be5ce1ac1c807eb05ae7ad8f010ca5?pvs=21)
2. [Immediate Opportunity](https://www.notion.so/ZK-Proof-Supply-Chain-Mapping-the-Race-very-simplified-mostly-Delphi-Reports-RiskZero-Taiko-S-18be5ce1ac1c807eb05ae7ad8f010ca5?pvs=21)
3. [Market Context: Tipping Point](https://www.notion.so/ZK-Proof-Supply-Chain-Mapping-the-Race-very-simplified-mostly-Delphi-Reports-RiskZero-Taiko-S-18be5ce1ac1c807eb05ae7ad8f010ca5?pvs=21)
4. [Proof Supply Chain](https://www.notion.so/ZK-Proof-Supply-Chain-Mapping-the-Race-very-simplified-mostly-Delphi-Reports-RiskZero-Taiko-S-18be5ce1ac1c807eb05ae7ad8f010ca5?pvs=21)
5. [Ecosystem](https://www.notion.so/ZK-Proof-Supply-Chain-Mapping-the-Race-very-simplified-mostly-Delphi-Reports-RiskZero-Taiko-S-18be5ce1ac1c807eb05ae7ad8f010ca5?pvs=21)
6. [Hardware](https://www.notion.so/ZK-Proof-Supply-Chain-Mapping-the-Race-very-simplified-mostly-Delphi-Reports-RiskZero-Taiko-S-18be5ce1ac1c807eb05ae7ad8f010ca5?pvs=21)
7. [Sources](https://www.notion.so/ZK-Proof-Supply-Chain-Mapping-the-Race-very-simplified-mostly-Delphi-Reports-RiskZero-Taiko-S-18be5ce1ac1c807eb05ae7ad8f010ca5?pvs=21)

---

# **Executive Summary**

- **ZK adoption in 2025** hinges on abstraction layers (zkVMs) replacing custom circuit development, unlocking use cases like privacy-preserving oracles, co-processors, and verifiable Bitcoin L2s.
- **Proof supply chain ecosystems** are fragmenting into vertically integrated players (Risk Zero, Succinct) and decentralized prover markets (Fermah, zkCloud), mirroring early AI GPU cloud dynamics.
- **Hardware innovation** reshapes economics: FPGAs dominate mid-term (3x cost efficiency vs. GPUs), while specific ASICs and VPUs promise 10x gains by 2026

---

# Immediate Opportunities

“At its core, blockchains require every single node to re-execute every transaction to achieve consensus. Think about that: thousands of nodes, all performing the exact same computation, over and over. This creates an endless cycle of redundant work that leads to massive limitations.

This model imposes brutal constraints on what’s possible onchain. Gas/compute limits strangle applications, forcing developers to optimize around scarcity rather than build for abundance. Complex computations remain impossible. The magic of blockchain – its ability to coordinate and compute trustlessly – remains locked behind arbitrary technical constraints. ***We will never bring the world onchain*** if we don’t solve this.

*This isn’t news*. Many teams have tried to solve this problem, creating new chains, L2s, and alternate scaling solutions. Don’t get me wrong – **these teams deserve immense credit for pushing the space forward**. But look where we’ve ended up: an ecosystem more fragmented than ever, with more chains than real-world use cases. We’re building more blockchains instead of upgrading the ones we have.

Zero-knowledge proofs emerged as our escape from this paradigm. ZK could eliminate re-execution entirely, transforming blockchains into the supercomputers they were meant to be. But two massive hurdles stood in our way:

1. Development barrier: ZK required cryptography expertise, and performance was too slow for real applications
2. Deployment barrier: ZK infrastructure was chain-specific and brutally complex to implement

Dozens of teams are tackling the first challenge head-on with the zkVMs. Instead of writing circuits, developers could just write Rust. No PhD required.” – [@zksanca](https://x.com/zksanca)

Currently, **the** Ethereum roadmap includes partial consensus transition to ZK tech according to Justin **Drake’s** Beam chain proposal and [Vitalik’s Ethereum Roadmap](https://x.com/ercwl/status/1856679876025303426).

![Снимок экрана 2025-02-03 в 14.03.58.png](ZK%20Proof%20Supply%20Chain%20Mapping%20the%20Race%20(very%20simpl%2018be5ce1ac1c807eb05ae7ad8f010ca5/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA_%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2025-02-03_%D0%B2_14.03.58.png)

By integrating ZK proofs (SNARKs / STARKs) in-protocol, full blocks could be verified without requiring all nodes to process every transaction.
Before full transition will happen several changes to Consensus Sublayer must happen.

**One of those changes is Chain Snarkification which is meant to reduce validator hardware dependency.**

**From consensus to EVM, Beam Chain will try to add zk to every module of the Ethereum protocol. There will be a zk EVM pre-compile that will simplify launching zk rollups, and developers won’t need to worry about bugs as the pre-compile will be enshrined in-protocol.**

### [**Ethproofs](https://ethproofs.org/) - is a public initiative that welcomes zkVM teams to verify Ethereum blocks, on the way to real time proving of the chain.**

- **Purpose**: Ethproofs is a credibly neutral dashboard that aggregates proving performance, cost, and latency for 1 out of 100 Ethereum blocks, provided by different zkVM teams. People can download the proofs and verify them themselves. Size, cycle and machine specifications of provers are also available.
- **Impact**: Forces zkVM teams to compete on efficiency, accelerating hardware-aware optimizations.
- **Current Status**:
    - **Snarkify (SP1)**, **ProjectZKM**, and **Succinct Labs** actively proving blocks.
    - Single-machine proofs prioritized for fairness; multi-machine support planned for Q2 2025 to reduce latency to **<12 seconds**.

<aside>
🚨

Everstake was invited by Snarkify to help them proof Ethereum blocks, as they plan to firstly onboard provers to this initiative. Should note that this is still a “public good”.

</aside>

<aside>
🚨

Risk Zero also invited us to participate in their closed testnet. Expected to run per party: at least 10 RTX 4090s. 

</aside>

---

# **Market Context: Tipping Point**

![Снимок экрана 2025-01-31 в 17.16.30.png](ZK%20Proof%20Supply%20Chain%20Mapping%20the%20Race%20(very%20simpl%2018be5ce1ac1c807eb05ae7ad8f010ca5/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA_%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2025-01-31_%D0%B2_17.16.30.png)

ZK research is getting the biggest boost in crypto, with massive capital and talent flowing in. We’re seeing validity proofs for zk-rollups, ZK light clients for bridging, and even Optimistic rollups—like Optimism, Arbitrum, Taiko, and Fuel—integrating zkVMs (Risc0, SP1 by Succinct and many more!) for hybrid proving. Beyond Ethereum, Solana’s leveraging ZK compression to manage state growth, and Sui’s zkLogin lets you create email-based wallets safely without giving up personal data.

![Снимок экрана 2025-01-31 в 17.21.17.png](ZK%20Proof%20Supply%20Chain%20Mapping%20the%20Race%20(very%20simpl%2018be5ce1ac1c807eb05ae7ad8f010ca5/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA_%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2025-01-31_%D0%B2_17.21.17.png)

Data from Our Network and [zkstats.io](http://zkstats.io/) shows ~1.6M proofs submitted on Ethereum since 2021, with total settlement fees (TSF) topping $60M. TSF(total settlement fees) peaked at $15M in Dec-23, driven by Linea, ZkSync, and Scroll. While these numbers seem modest, **proof generation and verification costs are becoming more efficient and lowering the costs 10x.** Most rollups now use recursive proof aggregation—where one ZKP verifies a batch of ZKPs—cutting down volume and fees on Ethereum - can be seen on the chart below.

Demonstrating usage of the aggregation integration:

![[https://l2beat.com/zk-catalog](https://l2beat.com/zk-catalog)](ZK%20Proof%20Supply%20Chain%20Mapping%20the%20Race%20(very%20simpl%2018be5ce1ac1c807eb05ae7ad8f010ca5/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA_%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2025-01-31_%D0%B2_17.27.47.png)

[https://l2beat.com/zk-catalog](https://l2beat.com/zk-catalog)

- **zkVM Democratization**: 70% of ZK projects now use generalized zkVMs (vs. 30% in 2024), slashing development time by 80% (Delphi Digital yearly report).
- **OP Rollups → ZK Rollups**: Migration accelerates as zkVM costs reach parity (e.g., Scroll’s **$0.03/proof** target by Q3 2025).
- **Interoperability**: AggLayer (Polygon) - probably the closest solution to solve L2 liquidity fragmentation and zkIBC (Celestia) unify liquidity via zk light clients, reducing fragmentation.

---

# Proof Supply Chain

As more rollups and applications rely on zkVMs for verifiable computing and privacy, the demand for ZK proofs is steadily rising. We’re seeing this uptick in demand already, and next-gen zkVMs—like R0, SP1, and Nexus—are poised to meet it by offering efficient and composable proving systems. These zkVMs tap into proof markets, which pool multiple prover networks (ASICs, GPUs, and other specialized hardware) to deliver proofs faster and cheaper.

With growing proof demand, proof markets benefit from economies of scale that drive down the marginal cost of generating each proof. This drop in costs could encourage provers to invest more in dedicated hardware—like VPUs (Verifiable Processing Units), ASICs, or GPUs. Thanks to recursive aggregation systems like Nebra, developers, rollups, and applications can increasingly lean on zkVMs for verifiable computing. As it becomes more standard rather than niche, demand for ZK solutions will only accelerate in the coming months and years.

With more requests flowing into proof markets, individual zkVMs and prover networks will continue seeking ways to improve efficiency. We can expect ongoing experimentation with cutting-edge proof systems, enhanced compression techniques, and advanced cryptographic primitives that streamline proof generation and verification. As zkVMs advance, barriers for developers will drop even further, encouraging broader adoption of zero-knowledge proofs across an ever-growing range of applications and rollups.

Proof markets like Fermah, Risc Zero’s Boundless, and Gevulot act as intermediaries, matching rollups and applications that need proofs with prover networks running zkVMs, zkEVMs, or custom circuits on specialized hardware. Through their mechanism design, they help set proof prices and foster competition among provers.

In this competitive environment, proof markets can develop strong advantages to protect their market share. Faster proof generation attracts more demand to a particular market, meaning provers stay active and see higher returns on their hardware investments. Proof markets that can accommodate a wide range of proof requirements drive even greater machine utilization, ultimately convincing provers to integrate where they can maximize their ROI.

- **Demand Side (Protocols & Apps):**
    - Blockchain infrastructure and off-chain applications need zero-knowledge proofs to secure or validate computations—examples include rollups, privacy solutions, or bridging protocols.
    - These projects (the “demand side”) must either build their own proof infrastructure or outsource it.
        
        ![Снимок экрана 2025-01-31 в 18.55.54.png](ZK%20Proof%20Supply%20Chain%20Mapping%20the%20Race%20(very%20simpl%2018be5ce1ac1c807eb05ae7ad8f010ca5/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA_%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2025-01-31_%D0%B2_18.55.54.png)
        
        ![Снимок экрана 2025-01-31 в 18.55.57.png](ZK%20Proof%20Supply%20Chain%20Mapping%20the%20Race%20(very%20simpl%2018be5ce1ac1c807eb05ae7ad8f010ca5/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA_%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2025-01-31_%D0%B2_18.55.57.png)
        
        ![Снимок экрана 2025-01-31 в 18.55.51.png](ZK%20Proof%20Supply%20Chain%20Mapping%20the%20Race%20(very%20simpl%2018be5ce1ac1c807eb05ae7ad8f010ca5/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA_%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2025-01-31_%D0%B2_18.55.51.png)
        
- **Supply Side (Provers & Infrastructure):**
    - Specialized operators run **compute infrastructure** (GPUs, FPGAs, ASICs) to generate proofs efficiently.
    - Some do this “in-house” (vertically integrated), while others rely on **proof marketplaces** (third-party services that handle the heavy lifting).
        
        ![Снимок экрана 2025-01-31 в 18.58.14.png](ZK%20Proof%20Supply%20Chain%20Mapping%20the%20Race%20(very%20simpl%2018be5ce1ac1c807eb05ae7ad8f010ca5/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA_%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2025-01-31_%D0%B2_18.58.14.png)
        
- **Aggregation & Verification Layers:**
    - **Aggregators** bundle transactions/operations that need proving.
    - **Verifiers** (smart contracts or off-chain services) check the validity of these proofs on-chain.
        
        ![Снимок экрана 2025-01-31 в 17.52.01.png](ZK%20Proof%20Supply%20Chain%20Mapping%20the%20Race%20(very%20simpl%2018be5ce1ac1c807eb05ae7ad8f010ca5/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA_%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2025-01-31_%D0%B2_17.52.01.png)
        

As more protocols require proofs, third-party “prover-as-a-service” platforms are emerging to meet the demand.

---

# Ecosystem

### Here is complete ZK market map made my Electric Capital in the middle of last year:

![Снимок экрана 2025-01-31 в 18.54.35.png](ZK%20Proof%20Supply%20Chain%20Mapping%20the%20Race%20(very%20simpl%2018be5ce1ac1c807eb05ae7ad8f010ca5/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA_%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2025-01-31_%D0%B2_18.54.35.png)

![Снимок экрана 2025-01-23 в 12.55.29.png](ZK%20Proof%20Supply%20Chain%20Mapping%20the%20Race%20(very%20simpl%2018be5ce1ac1c807eb05ae7ad8f010ca5/%25D0%25A1%25D0%25BD%25D0%25B8%25D0%25BC%25D0%25BE%25D0%25BA_%25D1%258D%25D0%25BA%25D1%2580%25D0%25B0%25D0%25BD%25D0%25B0_2025-01-23_%25D0%25B2_12.55.29.png)

Teams building bridges no longer need cryptography experts to craft custom circuits; they can tap into off-the-shelf zkVMs for easy proof generation. This spans all sorts of apps—light clients, oracles, bridges, KYC platforms—pretty much anything.

**Three key groups are set to capture a large slice of the ZK proving market:**

1. **Vertically Integrated Companies (e.g., Risc Zero)**
    - They build their own zkVM and maintain an internal proof market (like Risc Zero’s Boundless). A hypothetical oracle could plug into Risc0’s zkVM and generate proofs directly to Boundless.
    
    RiskZero’s vertical infrastructure includes following parts:
        - A verifiable execution environment (powered by zkVMs)
        - A decentralized marketplace (ensures reliable, cheap proofs)
        - Proof aggregation (makes verification affordable)
        - Universal settlement (verify on any chain)
        
        Together, these services provide everything needed to build and deploy ZK-powered applications.
    - Co-processors will likely also run ready-made zkVMs, so we will likely cover a wide range of applications.
2. **Separate Prover Networks (e.g., Fermah, zkCloud)**
    - They pool compute resources and feed them into the marketplaces above or serve standalone projects.
        
        ![Prover network versatility example.](ZK%20Proof%20Supply%20Chain%20Mapping%20the%20Race%20(very%20simpl%2018be5ce1ac1c807eb05ae7ad8f010ca5/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA_%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0_2025-01-28_%D0%B2_10.26.25.png)
        
        Prover network versatility example.
        
3. **High-Profile Players (e.g., Linea, Worldcoin, zkSync, Aztec)**
    - They may either outsource their proof generation or manage it in-house. We can cover them if source our compute to the versatile Prover Networks described above.
- **Separate note for Bitcoin L2s that might require zk technology:**
Risc Zero has already integrated Bitsnark for BTC verification, extending ZK verification to Bitcoin. Expect other vertically integrated marketplaces to follow suit, making a dedicated Bitcoin L2 sector focus unnecessary.

[Vertically integrated proof markets (demand  + supply side)](ZK%20Proof%20Supply%20Chain%20Mapping%20the%20Race%20(very%20simpl%2018be5ce1ac1c807eb05ae7ad8f010ca5/Vertically%20integrated%20proof%20markets%20(demand%20+%20supp%2018be5ce1ac1c81cf8e40c59c0b531719.csv)

[Proving Networks (can plug supply into any demand source)](ZK%20Proof%20Supply%20Chain%20Mapping%20the%20Race%20(very%20simpl%2018be5ce1ac1c807eb05ae7ad8f010ca5/Proving%20Networks%20(can%20plug%20supply%20into%20any%20demand%20%2018be5ce1ac1c819b9222f1d1cf42f485.csv)

[Big ZK L2s, infra (demand source)](ZK%20Proof%20Supply%20Chain%20Mapping%20the%20Race%20(very%20simpl%2018be5ce1ac1c807eb05ae7ad8f010ca5/Big%20ZK%20L2s,%20infra%20(demand%20source)%20190e5ce1ac1c815d8861d09a4de97bdd.csv)

---

# Hardware:

- **Recursive proof generation costs** will fragment hardware markets: GPUs dominate today (0.12$/proof), FPGAs (0.08$/proof) and ASICs (0.03$/proof) will potentially commoditize the supply chain by 2026 ([Pi2 Network](https://blog.pi2.network/zkvm-benchmarking/)).

**Paradigm**: 

> “We also expect FPGAs to outperform GPUs for similar reasons why they have thrived in machine learning and computer vision:
> 
- **Hardware Cost:** A top-of-class FPGA (leading process node, clock speed, energy efficiency, and memory bandwidth) is about 3x cheaper than a top-of-class GPU. The global demand for GPUs has further exacerbated this issue.
- **Power Efficiency:** FPGAs can be >[10x](https://docs.xilinx.com/v/u/en-US/wp492-compute-intensive-sys) more energy efficient than GPUs, a large reason being the requirement for GPUs to be connected to a host device, which is often consuming a lot of power”

**Risk Zero Boundless team**:

> “On-prem data centers can offer a 50%+ cost advantage. The endgame involves ASIC/FPGAs; AWS is unlikely to adopt quickly or price **competitively**”
> 

**Succinct founder Uma Roy**: 

> “The AI neo-clouds are very tailored for AI workloads. They all run H100s, which are not cost-efficient at all for ZK proving workloads.
> 

> I just see L40 {on Corewave} and the price is higher than AWS. Vast is not reliable enough for our workloads (at least the 4090s we tried).
> 

> Yes, H100s are too expensive and don’t give a sufficient performance boost to compensate {higher price}.”
> 

### Current leaders in hardware development:

[Ingonyama](https://www.ingonyama.com/): **library that helps accelerate GPU, CPUs to match ZKP benchmarks**

[Irreducible](https://www.irreducible.com/prover): **operate custom FPGA-accelerated server clusters tailor-made for cryptographic computation at scale**

[Cysic](https://cysic.xyz/products/asic-solutions): **selling zk tailored ASICs and offer GPU acceleration**

Below is a consolidated table comparing ASICs, FPGAs, GPUs, and VPUs for generating zero‑knowledge proofs (“proving”) based on publicly available benchmarks and industry reports (e.g. Pi2 Network’s zkVM benchmarks, Risk Zero’s on‑prem data, Delphi Digital’s Infra Report, and Fabric’s VPU documentation). Note that many numbers are context‑dependent (for example, whether one is measuring a “base” [non‑recursive] or recursive workload) and include overhead factors (energy, maintenance, and utilization inefficiencies). For clarity, the table focuses on non‑recursive “base” figures unless noted otherwise, with approximate values that many industry observers expect to improve further over the next few years.

### Hardware Comparison Table

| **Hardware** | **Estimated Cost per Proof (USD)** | **Throughput (Proofs/Min)** | **Energy Efficiency / Power** | **Maturity / Availability** | **Comments** |
| --- | --- | --- | --- | --- | --- |
| **GPU (e.g., A100)** | ~~$0.12 (recursive workload)*; lower in ideal base-case (~~$0.02) | ~25 (base, non‑recursive)~2.5 (recursive)** | Relatively high (e.g. ~300W); broadly available via cloud | Mature and widely deployed in data centers and the cloud | Widely accessible; however, when operating in recursive scenarios the cost and effective throughput drop substantially due to the inherent 10× slowdown in proof aggregation. Overheads (cooling, downtime, inefficiencies) are also factored in. |
| **FPGA** | ~$0.08 | ~30 (base, non‑recursive) | Lower power draw (e.g. ~50W); optimized for fixed tasks | Available in on‑premises; require specialized engineering | On‑prem FPGA clusters (e.g. as reported by Risk Zero) show about a 50% cost advantage over cloud GPU setups. They offer decent throughput with improved energy efficiency but demand more custom development effort. |
| **ASIC** | ~$0.05 – $0.10 (projected by 2026) | 50–80 (base, non‑recursive) | Very high efficiency; lowest power consumption | Emerging technology; prototypes exist with production scaling expected post‑2025 | ASICs are designed specifically for zk proof generation. Projections (e.g. from Delphi Digital and related sources) expect them to offer roughly 10× improvement over GPUs once mature, making them the most cost‑effective option in high‑volume scenarios. |
| **VPU (e.g., Fabric VPU)** | ~$0.05 (projected) | ~80 (base, non‑recursive estimate) | Extremely efficient; tailored for ZK-specific tasks | Early stage but promising; targeted for large-scale zk systems | VPUs are a specialized form of processor optimized for the arithmetic used in zk computations. They are expected to further reduce both latency and cost per proof compared to current ASIC projections, although market availability remains limited at this time. |
- The $0.12 per proof figure for GPUs includes conservative overhead factors such as energy inefficiencies, downtime, and additional operational costs that are common in cloud environments.
- * “Recursive” proof generation involves additional layers of computation (typically ~10× slower) compared to “base” non‑recursive proofs, thus lowering throughput and increasing the effective cost.

---

### Sources:

- [https://l2beat.com/zk-catalog](https://l2beat.com/zk-catalog)
- [https://www.ournetwork.xyz/p/on-261-zoomed-in-on-zero-knowledge-proofs](https://www.ournetwork.xyz/p/on-261-zoomed-in-on-zero-knowledge-proofs)
- [https://dune.com/nebra/zero-knowledge-proof-verification-cost-ethereum?ref=ournetwork.ghost.io](https://dune.com/nebra/zero-knowledge-proof-verification-cost-ethereum?ref=ournetwork.ghost.io)

[The Year Ahead for Infra 2025 - Delphi Digital.pdf](ZK%20Proof%20Supply%20Chain%20Mapping%20the%20Race%20(very%20simpl%2018be5ce1ac1c807eb05ae7ad8f010ca5/The_Year_Ahead_for_Infra_2025_-_Delphi_Digital.pdf)

- [https://x.com/zksanca/status/1872737546146308215](https://x.com/zksanca/status/1872737546146308215)
- [https://blog.pi2.network/zkvm-benchmarking/](https://blog.pi2.network/zkvm-benchmarking/)
- [https://ethproofs.org/](https://ethproofs.org/)
- [https://x.com/drakefjustin/status/1884885708399075464](https://x.com/drakefjustin/status/1884885708399075464)
- [https://blog.pi2.network/zkvm-benchmarking/](https://blog.pi2.network/zkvm-benchmarking/)

---

Similar to the race in AI on who’s LLM is more robust and less consuming we see race in developing zkVM from for-profit as well as from non-profit developers like a16z. All of the tech is open source and debated publicly. 

---

## Conclusion/CTA:

- **Join the Snarkification of Ethereum via Snarkify** – contribute to a public good aligned with the Ethereum roadmap:
    - Leverage marketing opportunities.
    - Stay updated on hardware requirements and trends in Ethereum’s zk ecosystem.
    - Enhance your dev ops team’s expertise for future operations in the zk market.
    - Build connections with early leaders in this emerging sector through your contributions.
- **Join the Risk Zero Testnet:**
    - Contribute using RTX 4090 GPUs (incentivization details are still unclear—further discussion with the team is recommended).