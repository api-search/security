---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: urbia.de
  spf: true
hosts:
- cert_expires: Oct  3 08:36:44 2026 GMT
  host: www.urbia.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urbia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Urbia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Urbia
provider_slug: urbia
slug: urbia-domain-security
source_filename: urbia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.urbia.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:36:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: urbia.de\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbia/refs/heads/main/security/urbia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Parenting
- Family
- Community
- Forums
- Pregnancy
- Media
- Germany
---
