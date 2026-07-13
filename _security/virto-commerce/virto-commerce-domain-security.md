---
api_specs:
- filename: VirtoCommerce.Catalog
  format: yaml
  label: Virto Commerce Catalog API
  slug: catalog
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Catalog
- filename: VirtoCommerce.Pricing
  format: yaml
  label: Virto Commerce Pricing API
  slug: pricing
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Pricing
- filename: VirtoCommerce.Inventory
  format: yaml
  label: Virto Commerce Inventory API
  slug: inventory
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Inventory
- filename: VirtoCommerce.Orders
  format: yaml
  label: Virto Commerce Order Management API
  slug: orders
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Orders
- filename: VirtoCommerce.Cart
  format: yaml
  label: Virto Commerce Shopping Cart API
  slug: cart
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Cart
- filename: VirtoCommerce.Customer
  format: yaml
  label: Virto Commerce Customer API
  slug: customer
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Customer
- filename: VirtoCommerce.Marketing
  format: yaml
  label: Virto Commerce Marketing API
  slug: marketing
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Marketing
- filename: VirtoCommerce.Quote
  format: yaml
  label: Virto Commerce Quotes API
  slug: quotes
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Quote
- filename: VirtoCommerce.Store
  format: yaml
  label: Virto Commerce Store API
  slug: store
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Store
- filename: VirtoCommerce.Platform
  format: yaml
  label: Virto Commerce Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://virtostart-demo-admin.govirto.com/docs/v3/VirtoCommerce.Platform
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: virtocommerce.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: virtocommerce.org
  spf: false
hosts:
- cert_expires: Sep 28 20:33:33 2026 GMT
  host: virtocommerce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 21:56:21 2026 GMT
  host: docs.virtocommerce.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 04:44:45 2026 GMT
  host: virtostart-demo-admin.govirto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Virto Commerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virto Commerce, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Virto Commerce
provider_slug: virto-commerce
slug: virto-commerce-domain-security
source_filename: virto-commerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: virtocommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:33:33 2026 GMT\n  hsts: null\n- host: docs.virtocommerce.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 21:56:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: virtostart-demo-admin.govirto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 04:44:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: virtocommerce.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: virtocommerce.org\n  dnssec: false\n  caa: []\n  spf:\
  \ false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/security/virto-commerce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B E-Commerce
- Catalog Management
- Order Management
- Pricing
- Inventory
- Shopping Cart
- Customer Management
- Marketing
- Payments
- Shipping
- Subscriptions
- Headless Commerce
- Open Source
- .NET
---
