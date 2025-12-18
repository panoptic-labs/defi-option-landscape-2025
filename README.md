# DeFi Options Landscape Report 2025

<p align="center">
  <img src="panoptic_banner.jpg" width="1000" title="Panoptic Banner"></img>

</p>

## Deployment

This repo exists to serve a PDF via GitHub Pages using Adobe's [PDF Embed API](https://developer.adobe.com/document-services/docs/overview/pdf-embed-api/gettingstarted/)

Currently, the ClientID for this and the sister repo (https://github.com/panoptic-labs/pips), are in the Adobe developer console for the user
`tarc@panoptic.xyz`, authenticated via "Sign in with Google"

To ensure deployment goes smoothly,

* Ensure in GitHub, in the "Settings" tab, that "Pages" is configured to deploy from a branch, that the branch is `main`, and that you have a custom domain set up with the desired domain (for this repo, it's "defioptions25.panoptic.xyz")
* Ensure the CNAME file in the repository has the correct subdomain (for this repo, it's "defioptions25")
* Ensure domain provider (at time of writing, CloudFlare) has the CNAME record for the correct subdomain (for this repo, it's Name: "defioptions25" and Target: "panoptic-labs.github.io")
* Ensure the Adobe Developer Console has a unique PDF Embed API Client ID for the subdomain. Unfortunately, Adobe requires one API Project and corresponding Client ID for each subdomain you want to use the PDF Embed API on.

After all this , push to main, and visit the desired domain. Ensure you can view the PDF on mobile too to confirm the API key is working correctly.

