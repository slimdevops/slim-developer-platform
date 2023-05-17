# Slim Developer Platform Changelog

Team Slim typically releases new features and functionality to our web portal, CLI, and APIs weekly. Bookmark this page and check frequently to get the latest. 

## Recent Releases

### May 12, 2023: Slim Portal

#### **Updated navigation**
Our new, scalable navigation makes it easy to find what you need throughout the Slim Platform. 

#### **Collections deprication**
We have deprecated our current Collections feature as part of a larger effort to more effectively surface the images you care about. Stay tuned for more updates. 

### April 6, 2023: Slim Portal

#### **Hardening by Layer**
We’ve added the ability to select ‘n’ and above layers to skip the hardening process when hardening an image. This will allow you to try out various levels of hardening to see which version of the hardened image works best in your production environment. This selection can be done in the CLI using the CLI flag --include-last-image-layers. 

#### **Improved onboarding**
We’ve updated our homepage to improve the onboarding experience. Now, you can connect your registry, scan images using Trivy and Grype, and begin the hardening process directly from our homepage launch pad. 

#### **Grype Scan Results** 
We’ve updated our method for pulling CVEs from the Grype database to ensure that we provide users with the most accurate CVE dataset (previously we pulled the largest CVE dataset from Grype). This will align Grype results on the Slim Platform with stand alone Grype results. 

#### **Downloadable Hardening Artifacts** 
With this release, you can now view, download, and select the hardening artifacts collected during the instrumentation phase of hardening. 

### March 31, 2023: Slim CLI: Version 0.0.13 
* ARM support for hardening images; use the --platform flag to set the correct platform for the instrumented and hardened images. 
* Generate vulnerability scans directly from the CLI using new vscan commands. 
* Hardening ease-of-use commands including the ability to list all hardening attempts for an image, list all runs for a hardening attempt, and download hardening artifacts. 

### March 24, 2023: Slim Portal

#### **Enhanced Vulnerability Scanning and SBOMs for Slim Hardened Images**

We’ve made it much easier to verify vulnerability reduction as a result of Slim's automated container hardening process. You can now run Trivy, Grype, Snyk, Prisma Cloud (Twistlock), or any 3rd-party scanner on your hardened images produced via Slim platform. You can also generate SBOMs using 3rd-party tools for these images with complete and accurate Package information. 

#### **Automatically generate CycloneDX SBOMs**

Slim automatically generates an SBOM every time it scans or hardens one of your images. You can download the SBOM directly from the [Packages](/docs/container-profile#packages) tab for the scanned image. We currently provide SBOMs in the [CycloneDX format](https://owasp.org/www-project-cyclonedx/), but other formats (including SPDX) are coming soon.

#### **Support for ARM images**

Attention Mac M-chip users! We now support profiling, instrumenting, and hardening for ARM-based containers. You will now be able to see ARM images in any Connected Registry and be able to [harden them via the Portal or CLI](/docs/automated-container-hardening). Note: This feature does not yet include cross-architecture (i.e., ARM to AMD) capabilities. Stay tuned for updates on multi-architecture improvements.

***
