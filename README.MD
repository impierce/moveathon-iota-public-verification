# Public verification of IOTA credentials

Our submission for the [IOTA Foundation's Moveathon](https://www.moveathon.build/europe) Europe edition.

This repository contains the complete codestack used in the demo using Git submodules.
It consists of the identity wallet UniMe, the company wallet UniTrust and the ssi-agent UniCore.

## The Team

- Sandro de Calonne (https://yummygum.com/)
- [Oran Dan](https://github.com/oran-dan) (https://www.impierce.com/)
- [Noah Kamphuisen](https://github.com/NoahMelle) (https://yummygum.com/)
- [Soula Andrikopoulos](https://github.com/nanderstabel) (https://www.impierce.com/)
- [Cheyenne Stutzriem](https://github.com/coplat) (https://www.impierce.com/)

## Project Overview

The public verification functionality is a breakthrough in the identity wallet world as we know it. So far credentials have always been trapped in ecosystems where at the minimum you need an identity wallet installed, if not have whole systems integrated, to partake in the viewing, validating and sharing of credentials. Our innovation will finally open the door for anyone and everyone wanting to see and validate someones credential(s), with the owners consent, without having to download anything or go through any hassle whatsoever.

We built a share button into our identity wallet UniMe, which will create a link ("Public Link") to the verify page on the Ecosystem Leader website of which the issuer of the shared credential is a member.

**Key Features**

- Simple, intuitive UI: your credential overview now simply has a share button added to the "three dots" menu button. This will take you immediately to the chosen media platform with the public verification link, and possible data, auto-filled. From the other anyone trying to see your credential now only needs to click your link, that's it. The link will take them to the verify page where they will see the credential, the issuer and even the verifier been validated live on the spot for them. They then also have all the information needed available to make their own judgement on top of the validation by going through the issuer profile, verifier profile and the credential information.

- Public Link management: The public link contains the url to the verify page with the Public Credential Access Token, a JWT, appended as a parameter. This token has its own status registered in a Token Status List which will be hosted on the IOTA mainnet using IOTA Notarization.

- Verify page: The public verification goes in 2 steps. The first page, the landing page will not yet display all information as to give the visitor an introduction into what its about to verify. The verifier will verify the Public Credential Access Token and then fetch the general, public information about the credential from the issuer. No personal data has yet been shared at this point. The visitor can then already get a chance to see if he wants to continue with the given information. When continuing to the next page the full verification process will be triggered. The Public Credential Access Token is then forwarded to the issuer. The issuer first verifies the verifier requesting the credential, then it verifies the Public Credential Access Token. If both check out, the actual credential is sent back. The verifier then verifies the credential and the issuer. All checks and information is then displayed to the visitor

## Getting Started

To go through the hosted demo flow you don't need to set up anything, which is the whole point of this demo.
- Install UniMe on your mobile from the internal Beta track in the App/Play store. Access to the internal Beta track is only granted upon request.
- Scan the QR code to get the EVC credential in your UniMe.
- Log into our LinkedIn demo account on your mobile. Login info is only granted upon request.
- Share the credential from your UniMe app. This will take you to LinkedIn and auto-fill the "add certification" form for you. You only have to click "add to profile".

You have now completed the "sharing" part of the flow.
For the final part of the demo you will switch to the verifier role. Let's say a recruiter looking around online for candidates for a certain vacancy. 
- Login to a different LinkedIn account, could be your own since no data will be shared or edited in this account.
- Go to the demo profile on LinkedIn
- Click on the link under the certification you just added to that profile
- Voila, instant verification of a credential without having to download any app or software, nor needing to have it implemented in any of your systems. The full verification experience publicly available and richly displayed.
