---
api_specs:
- filename: podium-s-api-workspace
  format: yaml
  label: Podium API
  slug: podium-api
  spec_type: Postman
  url: https://www.postman.com/podiumhq/podium-s-api-workspace
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: podium.com
  spf: true
hosts:
- cert_expires: Sep  4 12:15:18 2026 GMT
  host: www.podium.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 11:31:42 2026 GMT
  host: docs.podium.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 04:46:57 2026 GMT
  host: api.podium.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Podium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Podium, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Podium
provider_slug: podium
slug: podium-domain-security
source_filename: podium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.podium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 12:15:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.podium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 11:31:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.podium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:46:57 2026 GMT\n  hsts: null\ndomains:\n- domain: podium.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podium/refs/heads/main/security/podium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Communication
- Reviews
- Messaging
- Payments
- Webchat
- Local Business
- SMS
- Lead Generation
---
