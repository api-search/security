---
api_specs:
- filename: liquidonate-magicmatch-openapi.yml
  format: yaml
  label: MagicMatch by LiquiDonate
  slug: magicmatch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquidonate/refs/heads/main/openapi/liquidonate-magicmatch-openapi.yml
- filename: liquidonate-returnsdirect-openapi.yml
  format: yaml
  label: ReturnsDirect by LiquiDonate (Beta)
  slug: returnsdirect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquidonate/refs/heads/main/openapi/liquidonate-returnsdirect-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: liquidonate.com
  spf: true
hosts:
- cert_expires: Aug 22 02:02:50 2026 GMT
  host: www.liquidonate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 07:31:08 2026 GMT
  host: docs-magicmatch.liquidonate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 15:14:55 2026 GMT
  host: api.liquidonate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liquidonate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiquiDonate, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: LiquiDonate
provider_slug: liquidonate
slug: liquidonate-domain-security
source_filename: liquidonate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liquidonate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 02:02:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs-magicmatch.liquidonate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 07:31:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.liquidonate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:14:55 2026 GMT\n  hsts: null\ndomains:\n- domain: liquidonate.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquidonate/refs/heads/main/security/liquidonate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Reverse Logistics
- Returns Management
- Donations
- Nonprofits
- Retail
- Ecommerce
- Sustainability
- Circular Economy
- Shipping
- Supply Chain
- Excess Inventory
- Company
---
