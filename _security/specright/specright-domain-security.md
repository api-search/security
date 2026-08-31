---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: specright.com
  spf: true
hosts:
- cert_expires: Oct  5 22:39:04 2026 GMT
  host: www.specright.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: developer.specright.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: api.specright.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Specright Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Specright, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Specright
provider_slug: specright
slug: specright-domain-security
source_filename: specright-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.specright.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 22:39:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.specright.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.specright.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: specright.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/specright/refs/heads/main/security/specright-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Specification Management
- Supply Chain
- Packaging
- Product Lifecycle Management
- Manufacturing
- Sustainability
- Supplier Collaboration
- Bill of Materials
- Salesforce
- Enterprise Software
---
