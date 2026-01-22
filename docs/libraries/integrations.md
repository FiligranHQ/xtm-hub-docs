# OpenCTI Integrations Library

A comprehensive library of Integrations is available on the XTM Hub, providing seamless access to curated threat intelligence data. 

Currently, the library proposes CSV Feeds, TAXII Feeds, OpenCTI Streams, Third Party Integrations and Connectors.
Depending on the type of Integration, you can either use One Click Deploy or download and import it to OpenCTI platforms.

![Integrations library](../assets/images/integration-feeds-lib.png)

## Overview

The XTM Hub Integrations library represents a significant advancement in threat intelligence accessibility. 
The library features pre-built Integrations that have been curated by the Filigran team, 
ensuring high-quality, relevant threat intelligence data.

Organizations can benefit from one-click deployment capabilities that integrate directly with registered OpenCTI platforms, 
while maintaining completely free access without any cost barriers. 

Additionally, the platform supports public browsing, allowing users to explore available Integrations without requiring authentication.

## Getting Started

### Initial Subscription

Before accessing the full functionality of the Integrations library, 
your organization must complete a one-time subscription process. 

A designated person from your organization needs to subscribe to the library, 
which is completely free and serves as an enablement step for all subsequent users. 

Once this initial subscription is completed, all users from your organization will 
gain automatic access to the full range of services without any additional steps or recurring costs.

![Subscribe Integrations](../assets/images/subscribe-integrations.png)

### Accessing the Library

The XTM Hub provides two distinct access methods to accommodate different user needs.

Authenticated access offers the complete feature set, 
including the ability to browse and download Integrations, 
deploy feeds directly to OpenCTI platforms, 
and access detailed feed information and metadata. 

For users who prefer to explore before committing, 
public access provides read-only capabilities through the [Hub public portal](https://hub.filigran.io/), 
where the complete library catalog can be viewed along with feed descriptions and 
details without requiring any connection or subscription.

## Working with Integrations

### Feed Exploration

The XTM Hub provides comprehensive information when you interact with any Integration tile in the library. 
Each Integration includes detailed specifications and content descriptions to help you make informed decisions about Integration.

Download options are readily available for users who prefer manual import processes, 
while sharing capability allow you to generate shareable links that facilitate easy 
collaboration with team members and external partners.

The Integrations library offers several filters to help you find the feed that best suits your needs.
You can filter feeds by:

- Use case
- Integration Feed type (CSV Feed, Connector, etc.)
- Platform compatibility (with registered OpenCTI platforms)
- Deployment mode (automatic or manual)

### Sharing and Collaborating

The XTM Hub facilitates seamless collaboration through its comprehensive sharing functionality.
Users can generate universal links for any Integration, enabling cross-organization sharing with partners,
clients, or team members without requiring recipients to maintain XTM Hub accounts.

This approach removes barriers to information sharing while maintaining the integrity and
accessibility of threat intelligence data across different organizational boundaries.

![Top right buttons](../assets/images/one-click-deploy.png)

### One-Click Deployment

The streamlined deployment process represents the most efficient method for integrating library feeds
into your OpenCTI platform (available from OpenCTI 6.7.10).

Before using this functionality, your OpenCTI platform must be properly registered in the XTM Hub (see [OpenCTI registration documentation](../user/opencti-registration.md)). 

The deployment process is straightforward: select your desired compatible Integration tile, click on the ```Deploy on OpenCTI``` button, 
choose your target platform if multiple platforms are registered, 
and wait a few seconds until successful Integration is confirmed in your OpenCTI platform. 
That will open the import drawer, and you must fill the required information to deploy the Integration.

One click deployment is currently available for

- CSV Feeds
- TAXII Feeds
- Connectors

## Specific feed type considerations

### Manual Import Integrations to OpenCTI

Organizations that prefer traditional import methods can
easily download desired Integration from the library and manually integrate them
into their OpenCTI platforms. This process involves downloading the Integration file,
navigating to your OpenCTI platform, and using the standard Import functionality
to upload and configure the Integration according to your specific requirements.

### Connectors Compatibility

If you don’t know what a connector is you can check this link for further information:
[OpenCTI Connectors Documentation](https://docs.opencti.io/latest/deployment/connectors/)

All CSV feeds are compatible with every OpenCTI version, whereas Connectors require a minimum product version. 
You can verify whether a Connector is compatible with your registered platforms on both the Connector card:

![Connector card incompatibility tooltip](../assets/images/connector-card-incompatibility-tooltip.png)

And the Connector details page:

![Connector details incompatiblity warning](../assets/images/connector-details-incompatibility-warnings.png)

By hovering over the Connector version, you can see which platform needs to be updated to deploy that Connector.

The Connector card and Connectors details page also indicates whether the Connector supports automatic deployment.

![Connector card automatic deploy](../assets/images/connector-card-automatic-deploy.png)
![Connector details automatic deploy](../assets/images/connector-details-automatic-deploy.png)

## Technical Requirements and Best Practices

Successful Integration with the XTM Hub requires attention to several technical considerations. 
Users deploying feeds must maintain appropriate OpenCTI permissions, 
including UPDATE/CREATE capability for CSV Feeds, TAXII Feeds, OpenCTI Streams, Third Party Integrations or Connectors. 
Platform registration involves registering OpenCTI platforms in the XTM Hub.
