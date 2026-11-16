## 19.0.1.0.0 (local port / 2026-11-16)

- Tests tagged ``post_install`` / ``-at_install``: at install time
  ``purchase_stock`` may not be in the registry yet, but the DB already
  has NOT NULL ``picking_type_id``. Creating a PO without the field then
  fails; with the field passed too early Odoo raises ``Invalid field``.
- Resolve incoming ``picking_type_id`` via ``stock.picking.type`` /
  warehouse when needed.
