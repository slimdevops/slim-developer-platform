# Slim Developer Platform Changelog

Team Slim typically releases new features and functionality to our web portal, CLI, and APIs weekly. Bookmark this page and check frequently to get the latest. 

## Recent Releases

### March 24, 2023: Slim Portal

#### **Enhanced Vulnerability Scanning and SBOMs for Slim Hardened Images**

We’ve made it much easier to verify vulnerability reduction as a result of Slim's automated container hardening process. You can now run Trivy, Grype, Snyk, Prisma Cloud (Twistlock), or any 3rd-party scanner on your hardened images produced via Slim platform. You can also generate SBOMs using 3rd-party tools for these images with complete and accurate Package information. 

#### **Automatically generate CycloneDX SBOMs**

Slim automatically generates an SBOM every time it scans or hardens one of your images. You can download the SBOM directly from the [Packages](/docs/container-profile#packages) tab for the scanned image. We currently provide SBOMs in the [CycloneDX format](https://owasp.org/www-project-cyclonedx/), but other formats (including SPDX) are coming soon.

#### **Support for ARM images**

Attention Mac M-chip users! We now support profiling, instrumenting, and hardening for ARM-based containers. You will now be able to see ARM images in any Connected Registry and be able to [harden them via the Portal or CLI](/docs/automated-container-hardening). Note: This feature does not yet include cross-architecture (i.e., ARM to AMD) capabilities. Stay tuned for updates on multi-architecture improvements.

***
