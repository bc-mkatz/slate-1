## <span class="jumptarget"> List Shipping Methods </span>

Gets the list of shipping methods. (Default sorting is by shipping-method id, from lowest to highest.)

*   OAuth
>`GET /stores/{store_hash}/api/v2/shipping/zones/{id}/methods`

## <span class="jumptarget"> Get a Shipping Method </span>

Gets a shipping method.

*   OAuth
>`GET /stores/{store_hash}/v2/shipping/methods/{id}`

```json
{
  "id": 1,
  "name": "Australia Post",
  "method_name": "shipping_auspost"
}
```
