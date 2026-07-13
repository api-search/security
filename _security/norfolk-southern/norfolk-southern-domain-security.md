---
api_specs:
- filename: norfolk-southern-shipment-status-api.yml
  format: yaml
  label: Norfolk Southern Shipment Status API
  slug: shipment-status
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/norfolk-southern/refs/heads/main/openapi/norfolk-southern-shipment-status-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nscorp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: norfolksouthern.com
  spf: true
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: developer.nscorp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: www.norfolksouthern.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: api.nscorp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Norfolk Southern Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Norfolk Southern, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Norfolk Southern
provider_slug: norfolk-southern
slug: norfolk-southern-domain-security
source_filename: norfolk-southern-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.nscorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: false\n- host: www.norfolksouthern.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nscorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nscorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: norfolksouthern.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/norfolk-southern/refs/heads/main/security/norfolk-southern-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Freight
- Logistics
- Railroad
- Shipping
- Transportation
- Fortune 500
---
