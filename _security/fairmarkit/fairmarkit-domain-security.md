---
api_specs:
- filename: fairmarkit-buyer-openapi.json
  format: json
  label: Fairmarkit Buyer Public API
  slug: fairmarkit-buyer-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-buyer-openapi.json
- filename: fairmarkit-supplier-openapi.json
  format: json
  label: Fairmarkit Supplier Public API
  slug: fairmarkit-supplier-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-supplier-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fairmarkit.com
  spf: true
hosts:
- cert_expires: Sep 29 21:13:57 2026 GMT
  host: www.fairmarkit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:24:43 2026 GMT
  host: developers.fairmarkit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: staging.fairmarkit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fairmarkit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fairmarkit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fairmarkit
provider_slug: fairmarkit
slug: fairmarkit-domain-security
source_filename: fairmarkit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fairmarkit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:13:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.fairmarkit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:24:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: staging.fairmarkit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fairmarkit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/security/fairmarkit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Procurement
- Sourcing
- Supply Chain
- Purchasing
- Suppliers
- RFQ
- RFP
- Spend Management
- Webhooks
---
