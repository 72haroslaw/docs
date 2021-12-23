# Miscellaneous scripting services reference

## services.config (`Shopware\Core\System\SystemConfig\Facade\SystemConfigFacade`)

The `config` service allows you to access the shop&#039;s and your app&#039;s configuration values.


### get()

The `get()` method allows you to access all config values of the store.
Notice that your app needs the `system_config:read` privilege to use this method.

#### Arguments

##### `key`: string


The key of the configuration value e.g. `core.listing.defaultSorting`.

##### `salesChannelId`: string|null

**Default**: null

The SalesChannelId if you need the config value for a specific SalesChannel, if you don&#039;t provide a SalesChannelId, the one of the current Context is used as default.


#### Return value

**Type**: `array|bool|float|int|string|null`



### app()

The `app()` method allows you to access the config values your app&#039;s configuration.
Notice that your app does not need any additional privileges to use this method, as you can only access your own app&#039;s configuration.

#### Arguments

##### `key`: string


The name of the configuration value specified in the config.xml e.g. `exampleTextField`.

##### `salesChannelId`: string|null

**Default**: null

The SalesChannelId if you need the config value for a specific SalesChannel, if you don&#039;t provide a SalesChannelId, the one of the current Context is used as default.


#### Return value

**Type**: `array|bool|float|int|string|null`





