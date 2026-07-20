---
api_specs:
- filename: arctic-wolf-ticket-api-openapi.json
  format: json
  label: Arctic Wolf Ticket API
  slug: arctic-wolf-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arctic-wolf/refs/heads/main/openapi/arctic-wolf-ticket-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: arcticwolf.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: arcticwolf.net
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: portal.arcticwolf.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: docs.arcticwolf.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: ticket-api.managedgw.us001-prod.arcticwolf.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arctic Wolf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arctic Wolf, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Arctic Wolf
provider_slug: arctic-wolf
slug: arctic-wolf-domain-security
source_filename: arctic-wolf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.arcticwolf.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.arcticwolf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ticket-api.managedgw.us001-prod.arcticwolf.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: arcticwolf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: arcticwolf.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arctic-wolf/refs/heads/main/security/arctic-wolf-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- Security Operations
- Threat Intelligence
- Ticketing
- Endpoint Security
- SOC
---
