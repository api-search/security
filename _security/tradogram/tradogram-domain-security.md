---
api_specs:
- filename: integrations
  format: yaml
  label: Tradogram API
  slug: tradogram-api
  spec_type: OpenAPI
  url: https://www.tradogram.com/software/integrations
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tradogram.com
  spf: true
hosts:
- cert_expires: Aug 16 21:10:36 2026 GMT
  host: www.tradogram.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 13:04:37 2026 GMT
  host: api.tradogram.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tradogram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tradogram, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tradogram
provider_slug: tradogram
slug: tradogram-domain-security
source_filename: tradogram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tradogram.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 21:10:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tradogram.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 13:04:37 2026 GMT\n  hsts: null\ndomains:\n- domain: tradogram.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradogram/refs/heads/main/security/tradogram-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Procurement
- Purchase Orders
- Supplier Management
- Spend Management
- Contracts
- Budgets
- Accounts Payable
- Sourcing
- Inventory
- Procure-to-Pay
---
