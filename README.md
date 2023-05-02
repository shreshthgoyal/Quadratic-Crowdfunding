<!-- PROJECT LOGO -->
<br />
<p align="center">
  <h1 align="center">Decentalised Quadratic Crowdfunding Platform</h1>
  <p align="center">
   We fund with the community.  For the community.
   <br />
  </p>
</p>
<p align ="center">
<img src="https://lh3.googleusercontent.com/pw/AM-JKLXEmIbJBJ9tbeph97J8U0DOEbDMs9B3v7xeXaBNFoGNKjFMRhlES6t8OJ4RGP9lyljZN_782h3HaWuZOoCWWIRYDo-kLQPsKw4rx5Felg52XcoJfjLmRGiIrlYwbNXxrONFV0t2sv5lTec4V--7SKoR=w1686-h948-no?authuser=0" alt="ethqf" border="0">
</p>
<br />

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary><br />
  <ol>
    <li>
      <a href="#about-the-project">What is Eth QF?</a>
      </li>
      <li>
      <a href="#screenshots">Screenshots</a>
      </li>
      <li>
         <a href="#video">Demonstration Video</a>
      </li>
    <li><a href="#features">Features</a>
    </li>
    <li><a href="#technologies-used">Technologies, Libraries and Packages Used</a>
    </li>
      <li><a href="#local-setup">Local Setup</a></li>
      <li><a href="#next">What Next?</a></li>
    <li><a href="#team">Team Members</a></li>
  </ol>
</details>


<div id="about-the-project" />

<!-- ABOUT THE PROJECT -->
# What is Eth QF?

[Eth QF](https://github.com/shreshthgoyal/QF) is a decentralised platform that enables crowdfunding for projects on Ethereum ecosystem. Eth QF provides projects funding through the concept of Quadratic Funding. We at Eth QF, fund the community for the community.

### Why Blockchain?

* **Time efficient :** Blockchain allows us to make the entire process decentralized, where neither of the parties has all of the power. Essentially, any project has a chance of gaining visibility and funding. It also solves the issue of fees. While blockchain maintenance costs money, it drastically reduces transaction fees. This reduces the cost of crowdfunding for creators and investors.
* **High availability and immediate provision:** Any project that uses a blockchain-based crowdfunding model has the potential to receive funding. Anyone with an internet connection can also contribute to those projects. Crowdfunders using blockchain technology would not have to worry about the "fraud" that has plagued modern-day crowdfunding projects.
* **Seamless payment :** Blockchain also removes the worry of the project owners of having their fund withdrawn. The owners can easily withdraw the amount whenever they need to.

### What is Quadratic Funding?

* **Quadratic Funding converts 1$ to 20$!!**

Quadratic investment is a concept that extends ideas from quadratic vote casting to a mechanism for investing.
The **matching pool** is at the heart of Quadratic funding.
A matching pool is a money pool that is provided by matching companions. Matching partners are businesses, individuals, or even protocols that assist with public goods tasks. The funds collected in the matching pool are used to multiply individual contributions to exceptional initiatives.

You can learn more about  Quadratic Funding [here](https://finematics.com/quadratic-funding-explained/).

### Why Quadratic Funding?

* **Community driven :** In Quadratic Funding, the algorithm used after each CLR Matching Round, checks the number of contributors who donated to a certain project, in layman terms, the higher the number of contributors higher will be the amount supported to a project.
* **Need of the hour :** Crowd funding schemes for public goods have a fundamental weakness- the match amount for a project is proportional to the sum of contributions it receives during a stipulated period of time, whereas if community has more demand for some project than the other, proportion should not be equal. CLR Matching solves this problem.

<div id="screenshots" />

# Screenshots

Screenshots of our DApp are added to [this link](https://photos.app.goo.gl/FBom3kopCPeWn3Pj7).

<div id="video" />

# Demonstration 

Demonstration of our Dapp is added to [this link](https://youtu.be/CSQNWNy3WfY). <br />
You can checkout the presentation [here](https://www.canva.com/design/DAE46RT2TfQ/0IAllAnk_whCgz3dIGhndg/view?utm_content=DAE46RT2TfQ&utm_campaign=designshare&utm_medium=link&utm_source=sharebutton). <br />
Our Project Workflow is added to [this link](https://app.milanote.com/1N2f911lxmcl1C?p=JnqtrMZqLIf).

<div id="features" />

<!-- GETTING STARTED -->
# Features
* Project Owners can list their projects on the website from their GitHub. GitHub OAuth has been implemented in our application via which owners can list their projects and give information about their project to prevent scams.
* When listing the projects and contributing to a project, users need to go through a reCaptcha V2, to ensure bot-free listing.
* Contributors can filter projects from the list through filters like Project title and Project category.
* Each project is allocated its own description page from where contributors can learn about the project and the owner before contributing.
* Before contributing to a specific project, contributors need to go through an OTP based authentication to validate their contribution and reduce the risk of bot contributions.
* To prevent sybil attack contributors can at max contribute 5 times before their phone number gets dismissed.
> If this project goes in production, instead of OTP based authentication system, we are planning to introduce Aadhar API for user validation, as Aadhar API is not availabe for free we resorted to OTP based authentication system.

>The Sybil Attack is a type of attack seen in peer-to-peer networks in which a node in the network actively operates multiple identities at the same time, undermining authority/power in reputation systems. The main goal of this attack is to gain the majority of network influence in order to carry out illegal (in terms of network rules and laws) actions in the system.

* If a user wants to be a sponsor and donate funds to matching pool for public goods, they can contribute ethers in the sponsor page. We have set an lower limit of 5 ethers, for a user to be a sponsor.
* All the sponsor addresses are displayed on the sponsor page.
* Matching rounds states are displayed on each page, to notify the users whether a matching round is going on or not.
* Only the manager can initiate and distribute funds collected in the matching round, when a certain limit of amount is connected in the pool.
* Each project owner can withdraw the amount collected whenever they want to, through the withdraw button.

<div id="technologies-used" />

# Technologies, Libraries and Packages Used

1. ReactJS + Hooks
2. Ethereum
3. Solidity
4. Truffle
5. MetaMask
6. Ganache
7. Web3
8. jQuery
9. Firebase 


<div id="local-setup" />

# Local Setup

> **Pre-Requisites**
> React
> Ganache 
> MetaMask
> Truffle
1. Fork this repository.
2. Clone the repository
   ```sh
    git clone https://github.com/shreshthgoyal/QF.git
    ```
3. Open the folder in which you cloned the repository.
4. Open Ganache to run your local blockchain.
5. Run this command to build your smart contracts.
    ```sh
    truffle init
    truffle test
    truffle migrate --reset
    ```
6. Update your config.js present in root directory using abi and address present in build files.
7. Run on your local host and connect your wallet with metamask to perfrom the transactions.
8. To start your application run the following command in your terminal.
   ```sh
   npm start
   ```
   

> Star this repository ✨ or send us some ethers at 0x08C5374DfB9Df1A5D42C76a00AcA277CF98ABe50

<div id="next" />

# What Next?

* We can create a local IPFS gateway to store the files and create CIDs.
* We can have user profile system for project managers.
* We can have a archive feature where we can show history of previous Matching Rounds.

