# tslint-config

How to use this styleguide?

## Configuration

copy `.prettierrc` and `tslint.json` to your root directory 

## Dependencies

```
npm install prettier tslint tslint-config-prettier tslint-plugin-prettier tslint-sonarts typescript --save-dev
```

## CI Integration

execute the following command to generate the report with all errors

```
tslint -t json -o report.json --project .
```

Add the following to the sonar configuration.

```
sonar.typescript.tslint.reportPaths=report.json
```