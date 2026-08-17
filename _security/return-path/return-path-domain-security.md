---
api_specs:
- filename: return-path-everest-api-openapi.yml
  format: yaml
  label: Everest API
  slug: everest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/openapi/return-path-everest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: returnpath.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: validity.com
  spf: true
hosts:
- cert_expires: Sep 29 12:53:58 2026 GMT
  host: www.returnpath.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 05:08:13 2026 GMT
  host: developer.everest.validity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.everest.validity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Return Path Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Return Path, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Return Path
provider_slug: return-path
slug: return-path-domain-security
source_filename: return-path-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.returnpath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:53:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.everest.validity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 05:08:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.everest.validity.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: returnpath.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: validity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/security/return-path-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Martech
- Email
- Email Deliverability
- Email Marketing
- Sender Reputation
- Inbox Placement
- Deliverability
- DMARC
- Email Authentication
- Email Validation
- Analytics
---
