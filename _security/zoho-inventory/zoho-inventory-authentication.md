---
api_key_in: []
api_specs:
- filename: batches.yml
  format: yaml
  label: Zoho Inventory API
  slug: zoho-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-inventory/refs/heads/main/openapi/batches.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zoho Inventory Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Zoho Inventory secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Zoho Inventory
provider_slug: zoho-inventory
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
    scopes: 4
  name: Zoho_Auth
  sources:
  - openapi/batches.yml
  - openapi/bills.yml
  - openapi/compositeitems.yml
  - openapi/contact-persons.yml
  - openapi/contacts.yml
  - openapi/credit-notes.yml
  - openapi/currency.yml
  - openapi/customer-payments.yml
  - openapi/delivery-challans.yml
  - openapi/inventoryadjustments.yml
  - openapi/invoices.yml
  - openapi/itemgroups.yml
  - openapi/items.yml
  - openapi/landedcosts.yml
  - openapi/locations.yml
  - openapi/moveorders.yml
  - openapi/organizations.yml
  - openapi/packages.yml
  - openapi/picklists.yml
  - openapi/pricelists.yml
  - openapi/purchaseorders.yml
  - openapi/purchasereceives.yml
  - openapi/putaways.yml
  - openapi/replenishment.yml
  - openapi/reporting-tags.yml
  - openapi/retainer-invoices.yml
  - openapi/salesorders.yml
  - openapi/salesreturns.yml
  - openapi/serialnumbers.yml
  - openapi/shipmentorders.yml
  - openapi/storagelocations.yml
  - openapi/tasks.yml
  - openapi/taxes.yml
  - openapi/transferorders.yml
  - openapi/unit_of_measurement.yml
  - openapi/users.yml
  - openapi/vendor-credits.yml
  type: oauth2
slug: zoho-inventory-authentication
source_filename: zoho-inventory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/batches.yml, openapi/bills.yml, openapi/compositeitems.yml, openapi/contact-persons.yml,\n  openapi/contacts.yml, openapi/credit-notes.yml, openapi/currency.yml, openapi/customer-payments.yml,\n  openapi/delivery-challans.yml, openapi/inventoryadjustments.yml, openapi/invoices.yml, openapi/itemgroups.yml\n  ...\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: Zoho_Auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    scopes: 4\n  sources:\n  - openapi/batches.yml\n  - openapi/bills.yml\n  - openapi/compositeitems.yml\n  - openapi/contact-persons.yml\n  - openapi/contacts.yml\n  - openapi/credit-notes.yml\n  - openapi/currency.yml\n  - openapi/customer-payments.yml\n  - openapi/delivery-challans.yml\n  - openapi/inventoryadjustments.yml\n  - openapi/invoices.yml\n  - openapi/itemgroups.yml\n  - openapi/items.yml\n  - openapi/landedcosts.yml\n\
  \  - openapi/locations.yml\n  - openapi/moveorders.yml\n  - openapi/organizations.yml\n  - openapi/packages.yml\n  - openapi/picklists.yml\n  - openapi/pricelists.yml\n  - openapi/purchaseorders.yml\n  - openapi/purchasereceives.yml\n  - openapi/putaways.yml\n  - openapi/replenishment.yml\n  - openapi/reporting-tags.yml\n  - openapi/retainer-invoices.yml\n  - openapi/salesorders.yml\n  - openapi/salesreturns.yml\n  - openapi/serialnumbers.yml\n  - openapi/shipmentorders.yml\n  - openapi/storagelocations.yml\n  - openapi/tasks.yml\n  - openapi/taxes.yml\n  - openapi/transferorders.yml\n  - openapi/unit_of_measurement.yml\n  - openapi/users.yml\n  - openapi/vendor-credits.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-inventory/refs/heads/main/authentication/zoho-inventory-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Inventory Management
- Warehousing
- Sales Orders
- Purchase Orders
- Stock Adjustment
- Shipments
- Items
- E-commerce
---
