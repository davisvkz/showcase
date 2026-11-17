# Architecture

The shop has four parts that mirror each other:

1. **Models** — [Entity](../web/src/models/Entity.ts) is the base of
   [Product](../web/src/models/Product.ts) and [Order](../web/src/models/Order.ts).
2. **Pricing** — [PricingService](../web/src/services/PricingService.ts) on the web,
   [price.rs](../server/src/domain/price.rs) in Rust, [pricing.py](../tools/shop/pricing.py)
   in Python and [pricing.go](../service/internal/pricing/pricing.go) in Go.
3. **Storage** — [Repository](../web/src/services/Repository.ts) and
   [store.go](../service/internal/store/store.go).
4. **UI** — [App](../web/src/ui/App.tsx) renders the product list.

Back to the [README](../README.md). Configuration lives in
[the schema](../config/schema.json).

```text
This fenced link is ignored: [nothing](../README.md)
```
