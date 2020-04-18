# solhint-plugin-example

A minimal example showing how to write a plugin for [Solhint](https://github.com/protofire/solhint).

## Usage

Install solhint and this plugin:

```
npm install solhint solhint-plugin-example
```

Add plugin to your `.solhint.json` and enable the rule:

```
{
  "plugins": ["example"],
  "rules": {
    "example/no-foos": "error"
  }
}
```

To test it out:

```
echo 'contract Foo {}' > Foo.sol
./node_modules/.bin/solhint Foo.sol
```
