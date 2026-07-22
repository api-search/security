---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vaunte.com
  spf: true
hosts:
- cert_expires: Oct  3 14:14:40 2026 GMT
  host: www.vaunte.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vaunte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vaunte, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vaunte
provider_slug: vaunte
slug: vaunte-domain-security
source_filename: vaunte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vaunte.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:14:40 2026 GMT\n  hsts: false\ndomains:\n- domain: vaunte.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vaunte/refs/heads/main/security/vaunte-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fashion
- Commerce
- Marketplace
- Resale
- Defunct
---
