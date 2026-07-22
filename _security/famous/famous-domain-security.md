---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amaze.co
  spf: true
hosts:
- cert_expires: Oct 13 22:31:48 2026 GMT
  host: amaze.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Famous Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Famous, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Famous
provider_slug: famous
slug: famous-domain-security
source_filename: famous-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amaze.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 22:31:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amaze.co\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/famous/refs/heads/main/security/famous-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Creator Economy
- Commerce
- Live Shopping
- Media
- Ecommerce
- Marketing
---
