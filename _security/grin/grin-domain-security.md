---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "awstrust.com"
  - 0 issue "starfieldtech.com"
  - 0 issuewild "starfieldtech.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: grin.co
  spf: true
hosts:
- cert_expires: Oct 21 22:53:42 2026 GMT
  host: grin.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 16:45:40 2026 GMT
  host: api.grin.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grin, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Grin
provider_slug: grin
slug: grin-domain-security
source_filename: grin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grin.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 22:53:42 2026 GMT\n  hsts: false\n- host: api.grin.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 16:45:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: grin.co\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issue \"starfieldtech.com\"\n  - 0 issuewild \"starfieldtech.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grin/refs/heads/main/security/grin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Influencer Marketing
- Creator Economy
- Creator Management
- Affiliate Marketing
- Marketing
- Social-Media
- E-Commerce
---
