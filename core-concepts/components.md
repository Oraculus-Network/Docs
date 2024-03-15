# Components

1. #### Trusted Execution Environment:

\


![](https://lh7-us.googleusercontent.com/CDrKCcgXcnF8XRT9VqmcFs9hwWE18zQwxsQ8ERpkfn8hCZs8irl5u5bnXt-ZJ1LLKvtsIPUPYSIpWdSv0mdfXOtYS\_8avGLimxTj42IstFTH65OMxst81ArSncp6f\_qKTosn3iPtt7ZdkoavjO8pldY)

\


Our workload operates within an SGX-enabled computing environment, also known as a Trusted Execution Environment (TEE), powered by Theta Edge Cloud. Leveraging attestation and cryptography, we embed a unique seed within the TEE, safeguarded from external exposure, including the host system itself. This seed, utilized to derive an ECDSA key, facilitates various tasks such as loading encrypted user data , ensuring the integrity of the entire system, and generating shared secrets. Notably, this key serves as the central ECDSA key accessible solely within the TEE of all participating Edge Cloud VMs, remaining inaccessible to us, the host machine, or any other external entity—akin to a cryptographic 'black hole.' This innovative mechanism extends a myriad of possibilities and capabilities to the current blockchain ecosystem.

\
\


2. #### Data Indexer and Access Control SideChain

\


The data indexing and access control will be done with the help of our own chain which will be a subchain on the theta metachain. All the data that is uploaded to the storage layer will be encrypted with the Shared-Key (Private key of Owner +  TEE's public key) and so the data can only be accessed inside the Trusted Execution environment.  The data indexing will help the network to keep track of where the data is and makes our architecture flexible so that it can use different storage providers.&#x20;

Access control is a set of permission on each piece of data that can only be changed by the owner of the data. This access control will be stored as a state inside our modified theta metachain node. This access control will be responsible for maintaining the ownership as well as historical origins of the data piece.&#x20;

&#x20;

3. #### Orchestrator

\


In our meta chain, we've implemented sophisticated orchestration logic directly within the chain itself, complemented by a trusted execution environment (TEE). This combination enables the dynamic allocation and de-allocation of SGX server capacity through the Theta edge cloud service. Essentially, the chain nodes autonomously make allocation decisions and leverage the TEE to execute these decisions. The allocation key necessary for placing orders or managing the edge cloud account is derived and exclusively accessible within the TEE, ensuring complete chain control. This guarantees that our platform can effectively scale to meet high-demand workloads in a decentralized manner, without dependence on any central orchestration service. Such independence from centralized control mitigates the risk of bias, unresponsiveness, or malicious behavior that could arise from centralized systems in the event of errors.

\


4. #### Storage Layer

\


In our architecture, data access control is natively stored on our chain, while the actual data is stored off-chain on web3 storage providers such as Theta EdgeStore and IPFS. This strategic outsourcing of data storage enables us to focus primarily on access control mechanisms, leveraging battle-tested solutions provided by these established platforms. Both Theta EdgeStore and IPFS utilize unique identifiers, akin to hashes, making data retrieval efficient and reliable. By harnessing these existing storage solutions, we streamline our development efforts while ensuring robust access control measures. This approach not only enhances scalability and flexibility but also&#x20;

\


\


5. #### Multichain Relayers

\


In our system, multichain relayers play a pivotal role in facilitating communication and data exchange between disparate blockchains. These relayers, deployed within a Trusted Execution Environment (TEE) via the Theta Edge Cloud, serve as intermediary programs responsible for listening to events and transmitting computed results to the target chain. By operating within TEEs, these relayers ensure the confidentiality and integrity of the data being transmitted, safeguarding against unauthorized access or tampering. Leveraging the capabilities of the Theta Edge Cloud enables efficient deployment and management of these relayers, enhancing the scalability and reliability of our system. Ultimately, these multichain relayers empower Oraculus to seamlessly provide services across different blockchain networks, fostering interoperability and driving innovation in decentralized applications and services.

\
\
