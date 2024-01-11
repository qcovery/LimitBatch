# LimitBatch
This module limits the number of IDs requested from the index per batch.  
Some indices allow only a certain number of IDs per request (e.g. the Findex allows a maximum of 50 IDs).

## Usage
Integrate the module in the `modules` directory of VuFind and activate it by adding `LimitBatch` to `VUFIND_LOCAL_MODULES`.  

The limit is set by the `record_batch_size` setting in the `[Index]`block of the `config.ini`. Set it like this in your local file:
```ini
[Index]
record_batch_size = 100
```
