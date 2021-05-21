# AWS_GreenGrass_component_vmagent
GreenGrass component for vmagent.

# Quickstart
```shell
export BINARY_LOCATION=<binary_location>
aws s3 sync bin/* s3://$BINARY_LOCATION
sed 's/<FILL_BINARY_LOCATION_HERE>/$BINARY_LOCATION' eu.dobrovolny.filip.vmagent-1.59.0.yaml
aws greengrassv2 create-component-version --inline-recipe fileb://recipes/eu.dobrovolny.filip.vmagent-1.59.0.yaml
```

# Copyright

VMAgent is an opensource tool provided under [Apache 2.0](LICENSE) License. https://github.com/VictoriaMetrics/VictoriaMetrics/tree/master/app/vmagent