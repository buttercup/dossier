# Buttercup Platform

The Buttercup platform is made up of many (mostly open-source) projects that serve very specific purposes. The bulk of them are written in **JavaScript**, with a couple here and there written in **TypeScript**. There are also the odd instances of other languages, but these items are usually present to provide some native OS-level functionality.

The majority belong to the [Buttercup organisation](https://github.com/buttercup), though some individual projects referenced here are standalone.

## Project Tree

The core/shared structure (not exhaustive) of most Buttercup apps:

 * Buttercup Apps (desktop/mobile/web/terminal)
   * [Buttercup core](https://github.com/buttercup/buttercup-core) - Core functionality for the entire platform (Groups and Entries, Archives and Archive Managers etc.)
     * [iocane](https://github.com/perry-mitchell/iocane) - Encryption toolkit for NodeJS and the web
     * [WebDAV client](https://github.com/perry-mitchell/webdav-client) - WebDAV connection client
     * [Google Drive client](https://github.com/buttercup/googledrive-client) - Client for managing Google Drive files
     * [Dropbox client](https://github.com/buttercup/dropbox-client) - Client for managing Dropbox files
     * ~~[Datasources](https://github.com/buttercup/datasources) - Vault host adapters for connecting Buttercup to services like Dropbox, Google Drive etc.~~
     * ~~[Signing](https://github.com/buttercup/signing) - Encrypted string signing and validation~~
     * ~~[App-Env](https://github.com/buttercup/app-env) - Application environment bootstrap utility for preparing complex features like encryption for each specific platform (node/web, not React-Native)~~
     * ~~[Credentials](https://github.com/buttercup/credentials) - Login/token construct for transferring account credentails between core and the datasources~~
     * [Channel Queue](https://github.com/buttercup/channel-queue) - Procedure queuing for asynchronous tasks
   * ~~[Facades](https://github.com/buttercup/facades) - Object-only (serialisation) vault & entry handling~~
   * [Google OAuth2 client](https://github.com/buttercup/google-oauth2-client) - Authentication client for mapping user logins to OAuth2 tokens (offline access)
   
_NB: Struck-out items have most likely been recently included in the v4 release of Buttercup core._

**Browser extension:**

 * Extension
   * [Locust](https://github.com/buttercup/locust) - Login form detection and connection to Buttercup

**Desktop app:**

 * Desktop application
   * [Exporter](https://github.com/buttercup/buttercup-exporter) - Export Buttercup vaults
   * [Importer](https://github.com/buttercup/buttercup-importer) - Import vaults from other password managers
