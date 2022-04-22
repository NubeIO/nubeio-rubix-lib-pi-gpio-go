# nubeio-rubix-lib-pi-gpio-go


## api

Write all outputs at once (value from 0-100, for the 2x DOs 0=off 100=on)

```
http://0.0.0.0:5001/api/outputs/all/VALUE
```

Write on at a time (value from 0-100, for the 2x DOs 0=off 100=on)

POST
```
http://0.0.0.0:5001/api/outputs
```

BODY
Options for io_num ("UO1", "UO2", "UO3", "UO4", "UO5", "UO6", "DO1", "DO1")
```
{
    "io_num": "UO1",
    "value": 100,
    "debug": false
}
```




Get all input values
```
http://0.0.0.0:5001/api/inputs/all
```
