---
api_specs:
- filename: unfi-supplier-openapi.yml
  format: yaml
  label: UNFI Harmony Core API
  slug: unfi-harmony-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-natural-foods/main/openapi/unfi-supplier-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: unfi.com
  spf: true
hosts:
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: www.unfi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: suppliers.unfi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: api.unfi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: United Natural Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United Natural Foods (UNFI), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: United Natural Foods (UNFI)
provider_slug: united-natural-foods
slug: united-natural-foods-domain-security
source_filename: united-natural-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: suppliers.unfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.unfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: unfi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-natural-foods/refs/heads/main/security/united-natural-foods-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Food Distribution
- Wholesale
- Natural Foods
- Supply Chain
- Fortune 500
---
