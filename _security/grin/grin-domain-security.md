---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "godaddy.com"
  - 0 issue "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: grin.co
  spf: true
hosts:
- cert_expires: Aug 29 23:45:04 2026 GMT
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
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grin.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:45:04 2026 GMT\n  hsts: false\n- host: api.grin.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 16:45:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: grin.co\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grin/refs/heads/main/security/grin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Influencer Marketing
- Creator Economy
- Creator Management
- Affiliate Marketing
- Marketing
- Social Media
- eCommerce
---
