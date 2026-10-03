---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bandier.com
  spf: false
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: www.bandier.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bandier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bandier, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Bandier
provider_slug: bandier
slug: bandier-domain-security
source_filename: bandier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bandier.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: bandier.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bandier/refs/heads/main/security/bandier-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Fashion
- Retail
- E-Commerce
- Activewear
---
