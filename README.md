# validate-assets-open-config

This contains configuration for sbt-validate-assets.

#### Deprecated Dependencies

This is a json file containing the list of deprecated versions af asset libraries.
The file name is 'deprecated-dependencies.json'

The format is an array of JSON objects of the form:
```
{
  "assets": [{
    "key": "assets.version",
    "name": "assets-frontend",
    "range": "(,99.99.99)",
    "reason": "Update to latest versions",
    "from": "2099-01-01"
  }]
}
```

###### Where:

* _key_ and _name_ identify the dependency
* _range_ is used to declare minimum, maximum allowed versions of a dependency (both min and max may be optional), and allow "holes" for known incompatible versions. See 'Supported Version Ranges' for more details
* _reason_ tells why the versions in range are deprecated
* _from_ tells when the versions in range become unsupported.


##### Supported Version Ranges

Please see https://github.com/hmrc/sbt-validate-assets#supported-version-ranges
