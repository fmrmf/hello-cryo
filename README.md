# hello-cryo

A repo to try out [`cryo`](https://github.com/paradigmxyz/cryo).

## Setup

`cryo_python==0.2.0` fails to build given an older polars dependency, at least on my machine.
As a workaround, clone `cryo` into `src/`

```sh
cd src/vendor/
git clone https://github.com/paradigmxyz/cryo.git
```

Then build `cryo_python` locally with `maturin`

```sh
hatch shell
(hello-cryo) cd cryo/crates/python
(hello-cryo) maturin develop
```

`cryo_python` should now be installed into your `hatch shell` env.
