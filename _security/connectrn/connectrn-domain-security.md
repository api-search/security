---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: connectrn.com
  spf: true
hosts:
- cert_expires: Oct  3 18:45:32 2026 GMT
  host: www.connectrn.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: api.connectrn.com
  hsts: false
  http_status: 404
  https: true
  note: First-party application API host (AWS ALB). Returns a plain-text `NotFound` body on every probed path including `/`; no public documentation or contract.
  tls_version: TLSv1.3
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: app.connectrn.com
  hsts: true
  hsts_header: max-age=31536000; includeSubDomains
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: status.connectrn.com
  hsts: true
  hsts_header: max-age=31536000
  http_status: 200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Connectrn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConnectRN, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ConnectRN
provider_slug: connectrn
slug: connectrn-domain-security
source_filename: connectrn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.connectrn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:45:32 2026 GMT\n  hsts: false\n- host: api.connectrn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: false\n  http_status: 404\n  note: First-party application API host (AWS ALB). Returns a plain-text `NotFound`\n    body on every probed path including `/`; no public documentation or contract.\n- host: app.connectrn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_header: max-age=31536000; includeSubDomains\n  http_status: 200\n- host: status.connectrn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_header: max-age=31536000\n  http_status: 200\ndomains:\n- domain: connectrn.com\n  dnssec: false\n  caa: []\n  spf: true\n\
  \  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connectrn/refs/heads/main/security/connectrn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Health IT
- Staffing
- Nursing
- Workforce Management
- Marketplace
- Mobile App
---
