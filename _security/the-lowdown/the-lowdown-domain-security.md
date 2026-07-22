---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thelowdown.com
  spf: true
hosts:
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: thelowdown.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: The Lowdown Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Lowdown, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Lowdown
provider_slug: the-lowdown
slug: the-lowdown-domain-security
source_filename: the-lowdown-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thelowdown.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: thelowdown.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-lowdown/refs/heads/main/security/the-lowdown-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Women's Health
- Femtech
- Reproductive Health
- Contraception
- Digital Health
- Healthcare
- Consumer
---
