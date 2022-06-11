# how ZK proof work

[Zero Knowledge Proof (with Avi Wigderson) - Numberphile](https://www.youtube.com/watch?v=5ovdoxnfFVc)

[Open Vote Network for anonymous voting](https://github.com/stonecoldpat/anonymousvoting)

[Towards Smart Contract-based Verification of Anonymous Credentials](https://eprint.iacr.org/2022/492.pdf)

## zk-SNARK circut

[Create your first zero-knowledge snark circuit using circom and snarkjs](https://blog.iden3.io/first-zk-proof.html)
    
## Quadratic Arithmetic Program

[Quadratic Arithmetic Programs: from Zero to Hero](https://medium.com/@VitalikButerin/quadratic-arithmetic-programs-from-zero-to-hero-f6d558cea649)

[Stateless Clients: The Concept Behind](https://xord.com/research/stateless-clients-the-concept-behind/)

[Polynomial Commitments For Stateless Clients](https://xord.com/research/polynomial-commitments-for-stateless-clients/)

[Explaining Quadratic Arithmetic Programs](https://xord.com/research/explaining-quadratic-arithmetic-programs/)

# SNARK, STARK, winterfell, polygon miden

[zk-STARKS Explained by Quantstamp](https://www.youtube.com/watch?v=kk1Oo42TVQk)

[Polygon Miden - a STARK based ZK Rollup](https://www.youtube.com/watch?v=pLu7XeEN-f4)

[ElectAnon: A Blockchain-Based, Anonymous, Robust and
Scalable Ranked-Choice Voting Protocol
](https://arxiv.org/pdf/2204.00057.pdf)

[Semaphore](https://github.com/semaphore-protocol/semaphore) is a protocol, designed to be a simple and generic privacy layer for Ethereum DApps. Using zero knowledge, Ethereum users can prove their membership of a group and send signals such as votes or endorsements without revealing their original identity.

[whisper](https://eth.wiki/concepts/whisper/whisper-overview)

*note* : whisper is **depricated**
waku
https://rfc.vac.dev/spec/10/

waku have pool voting.
https://docs.wakuconnect.dev/docs/guides/vote_poll_sdk/
*note* : only **ERC-20** token holders can create or answer polls/votes.

*note* : In circut, doing string operations in your circuit definition is structurally wrong, IMO. Circuits should verify a relationship that you already know, using inputs pre-processed in order to be efficiently verifiable.
E.g. you would compute outside of the circuit that the string does indeed end with a substring, and then pass the position of that substring to the circuit in order for it to verify that fact.
