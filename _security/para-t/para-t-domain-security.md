---
api_specs:
- filename: para-t-openapi-original.yml
  format: yaml
  label: Paraşüt API V4
  slug: paraşüt-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/para-t/refs/heads/main/openapi/para-t-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: parasut.com
  spf: true
hosts:
- cert_expires: Sep 22 15:14:14 2026 GMT
  host: parasut.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 21:47:39 2026 GMT
  host: api.parasut.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Para T Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paraşüt, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paraşüt
provider_slug: para-t
slug: para-t-domain-security
source_filename: para-t-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parasut.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 15:14:14 2026 GMT\n  hsts: null\n- host: api.parasut.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 21:47:39 2026 GMT\n  hsts: null\ndomains:\n- domain: parasut.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/para-t/refs/heads/main/security/para-t-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Accounting
- Pre-Accounting
- e-Invoicing
- Invoicing
- Fintech
- SaaS
- Turkey
- ERP
- JSON:API
---
