# Rize Orb

This is the [Circle CI Orb](https://circleci.com/orbs/registry/) to 
generate a rize (shiny application) in a Docker container.
Please see the [published orb](https://circleci.com/orbs/registry/orb/vanessa/rize)
to get the latest version, or look into the [VERSION](VERSION) file here. 
The documentation will state 1.0.0 but we are beyond that version.

## Development

Before this Orb was used / tested with CircleCI, I needed to [install](https://circleci.com/docs/2.0/creating-orbs/)
the CircleCI client, and then validate it locally:

```bash
$ circleci orb validate src/orb.yml
```

and then create the namespace:

```bash
circleci orb create vanessa/rize
```

and also deployed a development alpha version

```bash
$ circleci orb publish src/orb.yml vanessa/rize@dev:alpha
```

For a vanilla CircleCI configuration (without the Orb) see [here](https://github.com/vsoch/rize-circle).
