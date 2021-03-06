# Client

Type: `class`

The Client class is the main class for this module and exposes different
endpoint classes to communicate with the Hetzner Cloud API.

## Functions

### \#constructor(opts)

| Parameter | Type                 | Description                                |
| --------- | -------------------- | ------------------------------------------ |
| opts      | `string` or `Object` | An API-Token or an Object (see below)      |

#### Passing an object

```javascript
// These are the default values. Replace them with yours!
const client = new HetznerCloud.Client({
  // API-Token (required)
  token: null,

  // Default base URL
  baseURL: 'https://api.hetzner.cloud/v1/',

  // Response timeout (5 seconds)
  timeout: 1000 * 5,

  // See "https://github.com/axios/axios#request-config" for more info
  proxy: false
})
```

## Properties

### .actions

An instance of [ActionsEndpoint](../endpoints/actions-endpoint.md)

### .servers

An instance of [ServersEndpoint](../endpoints/servers-endpoint.md)

### .floatingIPs

An instance of [FloatingIPsEndpoint](../endpoints/floatingips-endpoint.md)

### .sshKeys

An instance of [SSHKeysEndpoint](../endpoints/sshkeys-endpoint.md)

### .serverTypes

An instance of [ServerTypesEndpoint](../endpoints/servertypes-endpoint.md)

### .locations

An instance of [LocationsEndpoint](../endpoints/locations-endpoint.md)

### .datacenters

An instance of [DatacentersEndpoint](../endpoints/datacenters-endpoint.md)

### .images

An instance of [ImagesEndpoint](../endpoints/images-endpoint.md)

### .isos

An instance of [ISOsEndpoint](../endpoints/isos-endpoint.md)
