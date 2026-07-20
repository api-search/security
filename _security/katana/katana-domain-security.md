---
api_specs:
- filename: katana-openapi-original.json
  format: json
  label: Katana API
  slug: katana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/katana/refs/heads/main/openapi/katana-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: katanamrp.com
  spf: true
hosts:
- cert_expires: Oct  6 14:59:18 2026 GMT
  host: katanamrp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 16:47:25 2026 GMT
  host: api.katanamrp.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Katana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Katana, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Katana
provider_slug: katana
slug: katana-domain-security
source_filename: katana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: katanamrp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 14:59:18 2026 GMT\n  hsts: null\n- host: api.katanamrp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 28 16:47:25 2026 GMT\n  hsts: null\ndomains:\n- domain: katanamrp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/katana/refs/heads/main/security/katana-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Inventory
- Manufacturing
- ERP
- Supply Chain
- Warehouse Management
- Order Management
---
