# try-plaidml

## Quick start

See the [troubleshooting] section for solutions to common issues.

```
python3 -m venv plaidml-venv
source plaidml-venv/bin/activate
pip install plaidml-keras plaidbench
```

Choose which accelerator you'd like to use (many computers, especially laptops,
have multiple):

```
plaidml-setup
```

Next, try benchmarking MobileNet inference performance:

```
plaidbench keras mobilenet
```

Or, try training MobileNet:

```
plaidbench --batch-size 16 keras --train mobilenet
```
