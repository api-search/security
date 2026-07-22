---
api_specs:
- filename: wandera-risk-api-openapi.yml
  format: yaml
  label: Wandera RADAR Risk API
  slug: wandera-radar-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wandera/refs/heads/main/openapi/wandera-risk-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "geotrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wandera.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: jamf.com
  spf: true
hosts:
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: www.wandera.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 00:51:55 2026 GMT
  host: developer.jamf.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 10:33:54 2026 GMT
  host: api.wandera.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wandera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wandera, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wandera
provider_slug: wandera
slug: wandera-domain-security
source_filename: wandera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wandera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.jamf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:51:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wandera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 10:33:54 2026 GMT\n  hsts: null\ndomains:\n- domain: wandera.com\n  dnssec: false\n  caa:\n  - 0 issue \"geotrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: jamf.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wandera/refs/heads/main/security/wandera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Mobile Security
- Zero Trust
- Mobile Threat Defense
- Endpoint Security
- Device Risk
- Jamf
---
