---
description: ''
domains:
- caa:
  - 0 iodef "mailto:admin@cameo.com"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cameo.com
  spf: true
hosts:
- cert_expires: Aug  7 09:32:55 2026 GMT
  host: www.cameo.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cameo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cameo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cameo
provider_slug: cameo
slug: cameo-domain-security
source_filename: cameo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cameo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 09:32:55 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: cameo.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:admin@cameo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cameo/refs/heads/main/security/cameo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Video
- Marketplace
- Celebrity
- Entertainment
- Personalized Video
- Creator Economy
---
