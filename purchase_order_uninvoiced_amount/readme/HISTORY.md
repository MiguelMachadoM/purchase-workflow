## 19.0.1.0.0 (local port / 2026-11-16)

- Tests: remove ``uom.category`` creation (gone in Odoo 19 UoM model);
  use ``product.uom_id`` instead of ``uom_po_id``.
- ``post_install`` + explicit incoming ``picking_type_id`` for the same
  ``purchase_stock`` / at-install registry reason as other purchase ports.
