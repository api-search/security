---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org; cansignhttpexchanges=yes"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@highspot.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: highspot.com
  spf: true
hosts:
- cert_expires: Sep 25 21:18:00 2026 GMT
  host: www.highspot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: api-su2.highspot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Highspot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Highspot, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Highspot
provider_slug: highspot
slug: highspot-domain-security
source_filename: highspot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.highspot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 21:18:00 2026 GMT\n  hsts: false\n- host: api-su2.highspot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: highspot.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org; cansignhttpexchanges=yes\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@highspot.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highspot/refs/heads/main/security/highspot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sales Enablement
- Content Management
- Pitch Analytics
- CRM Integration
- Buyer Engagement
- Training
- Coaching
- AI
- MCP Server
---
