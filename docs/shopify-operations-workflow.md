# Shopify Operations Workflow

**Status:** Operating framework based on Timothy Nesmith's documented PhillyScreen e-commerce experience. It does not expose customer data or store credentials.

## Order flow

1. **Product setup:** confirm title, variants, price, cost, weight, product image, and fulfillment responsibility.
2. **Inventory check:** verify available stock or production lead time before promoting the item.
3. **Order review:** check variant, quantity, delivery method, customer note, and fraud or address exceptions through the platform's normal controls.
4. **Production or pick:** move the order into the production queue or pick from finished inventory.
5. **Quality gate:** compare product, size, decoration, and quantity with the order.
6. **Pack and fulfill:** record tracking or pickup confirmation and mark the order fulfilled only after handoff.
7. **Exception handling:** contact the customer through approved store channels when inventory, artwork, or address issues prevent fulfillment.
8. **Closeout:** reconcile product cost, shipping, refunds, and remaining inventory weekly.

## Management reports

- Open orders by age
- Units by product and variant
- Inventory below reorder point
- Gross margin by product group
- Refund and exception reasons
