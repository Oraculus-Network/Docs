# Innovation

\


1. #### Shared Secret

\


![](https://lh7-us.googleusercontent.com/vqDgxUQxiXnvTXH8bHblENIho\_K52uvkwRSjpcsvDRVJbfvp9lTDqGnOlDMb3Nz6Z9KoaZWB4irxvHC1j2HrYaQkJGCgODl60\_JWm9FJPjA1ZDiSkydUJ\_Dv7zzldv0d04IYb7Er4PaMYJUDy7eUaHw)

Properly utilizing a unique cryptographic mechanism, our system ensures that encrypted data can only be decrypted by the user and the TEE environment. This approach empowers autonomous processing and action-taking on the blockchain, imbued with access control, without dependency on any single entity. At its core, we employ Elliptic-curve Diffie-Hellman (ECDH) and AES, fortified by TEE attestation.

\


2. #### Trustable chain data inside tee

\


As a trusted execution environment (TEE) depends on an on-chain state to initiate specific execution flows, acquire permission data, or retrieve certain states from the chain. If the TEE relies solely on a single chain node, and that node happens to be compromised, it could lead to breaches of data integrity or disregarding data permission mechanisms. To address this, we incorporate algorithms akin to Chainlink's Off-Chain Reporting (OCR). Furthermore, considering the potential threat of a malicious host operating system within the TEE, we implement cryptographic signature mechanisms to safeguard the TEE from such risks.

\


3. #### Condition Evaluation on Private Data

Performing condition evaluations on private data without compromising its confidentiality is a critical aspect of privacy-preserving computation. Trusted Execution Environments (TEEs) offer a robust solution by providing secure enclaves where computations can be conducted while keeping the data encrypted and inaccessible to unauthorized entities. Within the TEE, encrypted data undergoes secure evaluation processes, ensuring that the condition is assessed without exposing the underlying sensitive information. Once the evaluation is complete, only the result of the computation is extracted from the TEE, maintaining the privacy of the original data. Optionally, zero-knowledge proofs can be employed to further enhance privacy assurances by verifying the correctness of the computation without revealing any details about the private data itself. This approach enables organizations to derive insights and make informed decisions based on private data without compromising confidentiality, ensuring compliance with privacy regulations and safeguarding sensitive information from unauthorized access.

\
\


4. #### Data NFT

\


Introducing a novel concept: the Data NFT. With a Data NFT, the owner exclusively gains access to the data or its utilization within specific applications executed within the TEE. Additionally, the owner can grant permissions for others to conduct checks on this data and derive outcomes. The submission of outcomes to the chain is confined to execution solely within the TEE, ensuring that the executor can only provide logic for verification without accessing the data itself. This innovation opens doors to numerous use cases.

\


5. #### Secure Deployment

\


The Secure Deployment service, facilitated by SGX instances, ensures the secure deployment of services like Theta Edge Cloud. Integration of TPM enhances confidentiality and integrity, while Terraform enables consistent infrastructure deployment. Key management, leveraging TPM, prevents API key leaks. Verifiability is assured through cryptographic techniques like digital signatures and remote attestation. End-to-end encryption secures communication channels, and continuous monitoring detects and responds to threats promptly. With these measures, deployments are conducted securely, minimizing risks of key exposure and unauthorized access, thereby instilling trust in the deployment process.

\
