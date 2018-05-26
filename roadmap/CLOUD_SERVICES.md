# Cloud Services for storing Buttercup Archives

This document deals with Archive storage solutions provided by the Buttercup platform, which solutions may be added in the future, and which are blocked until further notice.

## Supported solutions

The following cloud storage providers are supported by the platform:

 * Dropbox
 * ownCloud
 * Nextcloud
 * WebDAV (see below)
 
### WebDAV operators

Not all WebDAV operators are supported. A whitelist is maintained here for those that are known to work well with Buttercup:

 * [Yandex](https://yandex.ru/)

## Greenlit solutions

These items have been OK'd for future integration:

 * Amazon Drive
 * Box
 * One Drive

## Blocked/Pending solutions

These items are **not to be implemented** until further notice. Merge-requests regarding these items may be closed without warning:

 * Google Drive
 * Hubic
 * Citrix ShareFile (Supports WebDAV)
 * Sync.com

These items may be blocked for one or more of the following reasons:

 * Insufficient public usage - We're responsible for the maintenance and upkeep of each provider Buttercup uses. We'll concentrate on the more popular services for now.
 * Questionable brand / platform stability
 * Incompatible or obscure API
 
