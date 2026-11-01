---
api_specs:
- filename: clara-com-mx-openapi-generated.yml
  format: yaml
  label: Clara API
  slug: clara-com-mx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clara-com-mx/openapi/_ae-authored/clara-com-mx-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clara.com.mx
  spf: true
hosts:
- cert_expires: Nov 24 21:29:19 2026 GMT
  host: www.clara.com.mx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clara Com Mx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clara, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clara
provider_slug: clara-com-mx
slug: clara-com-mx-domain-security
source_filename: clara-com-mx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clara.com.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 21:29:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clara.com.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/clara-com-mx/security/clara-com-mx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Corporate Cards
- Expense Management
- Accounts Payable
- Travel Pay
- AI Finance
- Latin America
- ERP Integration
---
