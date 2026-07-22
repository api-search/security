---
api_specs:
- filename: vinculum-eretail-openapi-original.yml
  format: yaml
  label: Vin eRetail API
  slug: vin-eretail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-eretail-openapi-original.yml
- filename: vinculum-sellerpanel-openapi-original.yml
  format: yaml
  label: Vin eRetail SellerPanel V3 API
  slug: vin-eretail-sellerpanel-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/openapi/vinculum-sellerpanel-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vinculumgroup.com
  spf: true
hosts:
- cert_expires: Sep  7 18:48:52 2026 GMT
  host: www.vinculumgroup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vinculum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vinculum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Vinculum
provider_slug: vinculum
slug: vinculum-domain-security
source_filename: vinculum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vinculumgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 18:48:52 2026 GMT\n  hsts: null\ndomains:\n- domain: vinculumgroup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vinculum/refs/heads/main/security/vinculum-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Ecommerce
- Omnichannel
- Order Management
- Warehouse Management
- Inventory
- Retail
- Marketplaces
---
