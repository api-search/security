---
api_specs:
- filename: ch-robinson-worldwide-rest-apis-openapi.yml
  format: yaml
  label: C.H. Robinson Carrier API
  slug: carrier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ch-robinson-worldwide/refs/heads/main/openapi/ch-robinson-worldwide-rest-apis-openapi.yml
- filename: ch-robinson-worldwide-rest-apis-openapi.yml
  format: yaml
  label: C.H. Robinson Navisphere Shipper API
  slug: shipper-navisphere-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ch-robinson-worldwide/refs/heads/main/openapi/ch-robinson-worldwide-rest-apis-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chrobinson.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: navisphere.com
  spf: true
hosts:
- cert_expires: Oct  7 03:48:53 2026 GMT
  host: www.chrobinson.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:24:35 2026 GMT
  host: developer.chrobinson.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 16:45:44 2026 GMT
  host: sandbox-api.navisphere.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Ch Robinson Worldwide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for C.H. Robinson, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: C.H. Robinson
provider_slug: ch-robinson-worldwide
slug: ch-robinson-worldwide-domain-security
source_filename: ch-robinson-worldwide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chrobinson.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:48:53 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: developer.chrobinson.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:24:35 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: sandbox-api.navisphere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 16:45:44 2026 GMT\n  hsts: null\ndomains:\n- domain: chrobinson.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: navisphere.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ch-robinson-worldwide/refs/heads/main/security/ch-robinson-worldwide-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Freight
- Logistics
- Shipping
- Supply Chain
- Transportation
- Transportation Management
- Fortune 500
---
