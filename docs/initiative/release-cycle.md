# OpenEuropa Release Cycle
This document explains the release process followed by OpenEuropa project for its components.
OpenEuropa releases its component following semantic versioning (https://semver.org/)

There are three types of releases: 

- **MAJOR**: Incompatible API changes, very rare and planned in. 
- **MINOR**: Adds backwards-compatible manner functionalities and bug fixes.
- **PATCH**: Adds backwards-compatible bug/security fixes and can be deployed instantaneously. No new functionality will be introduced.

OpenEuropa components release plan don't follow a fixed overall timeline and can happen in different planned slots. Each component roadmap and release plan will be made available to the public.

## Release preparation and testing

The OpenEuropa team commits to have its components aligned with the API of the supported Drupal versions.

It is predicted that the majority of changes will come in the form of MINOR and PATCH releases. However, if there is a need to change API provided by the component in a way that it is not backwards compatible a new MAJOR release can be produced. 

Each OpenEuropa component defines in its dependencies the minimum requirements for components version it depends upon. Each minor version can have development, beta, and release candidate phases.

## Release support

For Drupal components, OpenEuropa team have a support policy inspired by Drupal core:
- Components support current and previous Drupal Core minor versions. New minor versions for components are made compatible with these respective core versions.
- When a new minor core version (n) is supported, the support for release n-2 is dropped. 

This follows a similar release cycle proposed for Drupal Core from a security standpoint and guarantees that all users of OpenEuropa components are running current minor release of supported Drupal Core (n) or previous (n-1).
As Drupal core minor releases happen every 6 months, website and application owners should be prepared to update to every minor release at least every 6 months.

## Backwards compatibility

Our Backward Compatibility Promise allows developers to upgrade with confidence from one minor version to the next one. Whenever keeping backward compatibility is not possible, the feature, the enhancement or the bug fix will be scheduled for the next major version.

## References
https://www.drupal.org/core/release-cycle-overview
