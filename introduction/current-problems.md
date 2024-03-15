# Current Problems

### Identifying Core Issues: Oraculus Originates from Fundamental Smart Contract Limitations

\
\


#### Limitations of Smart Contracts in Accessing Critical Data

\


Smart contracts, although foundational to powerful financial tools in Web3 like Uniswap, Aave, Compound, and Synthetix, can't directly access critical data. While these decentralized finance (DeFi) protocols have revolutionized markets by enabling trustless asset management, they lack the ability to incorporate dynamic, data-driven decision-making. For example, in platforms like Aave, both new borrowers and seasoned entities receive the same rate despite differences in on-chain assets and history.

\


Moreover, the utilization of private data in smart contracts for decision-making is currently unfeasible. Although there are oracle solutions available, they fail to ensure true isolation and trusted computing of data due to limitations in their infrastructure design. This limitation impedes the application of smart contracts in various scenarios such as insurance, credit scoring, and beyond.

\


#### Missed Opportunities: Smart Contracts and Sensitive Data Computation

\
\


Smart contracts, as executed on blockchain networks, indeed face significant limitations when it comes to performing computations on sensitive data without revealing the content of that data. This constraint stems from the fundamental design principles of blockchain technology, particularly its decentralized and transparent nature.

These limitations significantly restrict the types of use cases that can be effectively implemented using smart contracts. Many industries and applications require the ability to perform computations on confidential data, such as financial transactions, healthcare records, or supply chain logistics. Without a secure mechanism for processing this data within smart contracts, these use cases remain largely untapped within the blockchain ecosystem.

For example, in the healthcare industry, smart contracts could potentially streamline processes such as patient consent management, insurance claims processing, or clinical trials management. However, these applications require the ability to perform computations on sensitive patient data while preserving patient privacy and confidentiality. Without a secure solution for handling this data within smart contracts, the adoption of blockchain technology in healthcare remains limited.

Similarly, in the financial sector, there is growing interest in using blockchain technology for applications such as cross-border payments, trade finance, or asset tokenization. However, these applications often involve confidential financial data that cannot be safely processed within smart contracts without risking exposure to unauthorized parties.

In summary, while smart contracts offer many benefits in terms of transparency, immutability, and automation, their inability to perform computations on sensitive data without revealing its content presents a significant barrier to the adoption of blockchain technology in many industries. Addressing this challenge will require the development of secure cryptographic techniques and privacy-preserving protocols that enable smart contracts to operate on confidential data without compromising privacy or security. Until then, many potential use cases for blockchain technology will remain unrealized.

\


#### Lack of Autonomous Decision-Making in Smart-Contracts

\


The current landscape of smart contracts faces a significant challenge in the absence of event-driven functionality akin to web hooks, particularly concerning the context of users' accounts and private keys. Unlike traditional web development, where events trigger actions seamlessly, smart contracts lack the capability to automatically react to events occurring on other contracts. For instance, if a particular event transpired on smart contract X, there's no inherent mechanism for smart contract Y to autonomously respond without manual intervention from the user.

\


This limitation introduces inefficiencies and potential security risks. Users must actively monitor events across various contracts and execute corresponding functions manually, increasing the likelihood of errors or oversight. Additionally, the absence of automated reactions impedes the seamless integration of smart contracts into complex workflows and decentralized applications (dApps).

\


Furthermore, the reliance on manual intervention undermines the fundamental principles of decentralization, as it reintroduces centralized control points where users must intervene to facilitate interactions between contracts. This undermines the trustless nature of smart contracts and reduces the overall efficiency and scalability of decentralized systems.

\


Addressing this issue requires the development of innovative solutions that enable smart contracts to react automatically to events, empowering them to interact seamlessly with each other and with users' actions. Implementing event-driven functionality within the context of users' accounts and private keys would enhance the usability, security, and scalability of smart contract-based systems, paving the way for more sophisticated decentralized applications and ecosystems.

\
