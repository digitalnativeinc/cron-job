# @terra-money/houston-config

Utility for interacting with houston-config.js files

### Usage

```javascript
import HoustonConfig from "@terra-money/houston-config";
```

#### Instantiate default HoustonConfig object

```javascript
const newConfig = HoustonConfig.default();
```

#### Instantiate custom HoustonConfig object

```javascript
const customConfig = new HoustonConfig(
  "/houstonDirPath",
  "/currentWorkingDirPath",
  networkObj
);
```

#### Config.detect()

```javascript
// find config file & return new HoustonConfig object with config file settings (cwd)
const HoustonConfig = HoustonConfig.detect();

// find config file & return new HoustonConfig object from custom working dir
const HoustonConfig = HoustonConfig.detect({ workingDirectory: "./some/Path" });

// find & return new HoustonConfig object from custom named config
const customHoustonConfig = HoustonConfig.detect({}, "./customConfig.js");
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[Apache 2.0](https://choosealicense.com/licenses/apache-2.0/)