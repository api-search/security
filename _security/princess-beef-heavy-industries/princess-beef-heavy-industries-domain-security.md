---
api_specs:
- filename: princess-beef-heavy-industries-giftshop-openapi.yml
  format: yaml
  label: Pb33f Giftshop API
  slug: giftshop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princess-beef-heavy-industries/refs/heads/main/openapi/princess-beef-heavy-industries-giftshop-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pb33f.io
  spf: true
hosts:
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: pb33f.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 02:27:43 2026 GMT
  host: api.pb33f.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Princess Beef Heavy Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Princess Beef Heavy Industries, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Princess Beef Heavy Industries
provider_slug: princess-beef-heavy-industries
slug: princess-beef-heavy-industries-domain-security
source_filename: princess-beef-heavy-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pb33f.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: false\n- host: api.pb33f.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 02:27:43 2026 GMT\n  hsts: null\ndomains:\n- domain: pb33f.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/princess-beef-heavy-industries/refs/heads/main/security/princess-beef-heavy-industries-domain-security.yml
summary_line: TLSv1.3
tags:
- Commerce
- Documentation
- Editors
- Governance
- Platform
- Products
- Rules
---
