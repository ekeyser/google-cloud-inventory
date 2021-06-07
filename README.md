google-cloud-inventory
========

#### Google Cloud Infrastructure Inventory ####

This module provides an abstraction layer to inventory your cloud resources.

Supported services (and APIs):

Supported Regions

### Installation ###
```bash
npm install google-cloud-inventory
```

### Usage ###

```javascript
import GoogleCloudInventory from 'google-cloud-inventory'

const config = {
  credentials: {
    accessKeyId: 'your_access_key',
    secretAccessKey: 'your_secret_key'
  },
  services: ['ec2', 'rds'],
  regions: ['us-west-2, us-east-1']
};

const oInventory = new GoogleCloudInventory(config);
const oResources = oInventory.inventory();
```
