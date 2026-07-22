---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "www.digicert.com"
  - 0 iodef "mailto:security@taptapsend.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: taptapsend.com
  spf: true
hosts:
- cert_expires: Sep 28 22:35:46 2026 GMT
  host: taptapsend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taptapsend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taptap Send, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Taptap Send
provider_slug: taptapsend
slug: taptapsend-domain-security
source_filename: taptapsend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taptapsend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 22:35:46 2026 GMT\n  hsts: false\ndomains:\n- domain: taptapsend.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"www.digicert.com\"\n  - 0 iodef \"mailto:security@taptapsend.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taptapsend/refs/heads/main/security/taptapsend-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Money Transfer
- Remittances
- Fintech
- Payments
- Mobile Money
- Financial Services
---
