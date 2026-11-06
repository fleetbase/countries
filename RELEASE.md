> v0.9.0 ~ "Installs alongside Carbon 3 and Laravel 12"

---
## Highlights

- **`pragmarx/coollection` removed.** Its chain to `ia-collection` pinned `nesbot/carbon` to 1 or 2, which blocked every Laravel 12 release.
- **`Coollection` now lives in this package** as `PragmaRX\Countries\Package\Support\Coollection`, on top of `Illuminate\Support\Collection`, and `coollect()` is defined here.
- **Requires `illuminate/*` `^10` to `^13` and PHP 8.1 or later.** It also works on Laravel 10.
- **Tests run in CI**, across Laravel 10 and 12.

## Breaking

Code that type-hints `PragmaRX\Coollection\Package\Coollection` must move to the new class. `PragmaRX\Countries\Package\Support\Collection` keeps its name.

## Not tested

The data updater (`testUpdateCountries`) now needs `COUNTRIES_RUN_UPDATER=1` and wasn't run.
