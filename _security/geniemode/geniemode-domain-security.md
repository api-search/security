---
api_specs:
- filename: geniemode-cataloguing-api-swagger-2.0.json
  format: json
  label: Geniemode Cataloguing API
  slug: geniemode-cataloguing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geniemode/refs/heads/main/openapi/geniemode-cataloguing-api-swagger-2.0.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: geniemode.com
  spf: true
hosts:
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: geniemode.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: portal.geniemode.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Geniemode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geniemode, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Geniemode
provider_slug: geniemode
slug: geniemode-domain-security
source_filename: geniemode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geniemode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\n- host: portal.geniemode.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: geniemode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geniemode/refs/heads/main/security/geniemode-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sourcing
- Supply Chain
- Procurement
- B2B Commerce
- Manufacturing
- Logistics
- Textiles
- Apparel
- Furniture
- Quality Control
- India
---
