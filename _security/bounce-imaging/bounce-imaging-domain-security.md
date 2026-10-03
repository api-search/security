---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: bounceimaging.com
  spf: true
hosts:
- cert_expires: Nov 25 11:17:01 2026 GMT
  host: bounceimaging.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bounce Imaging Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bounce Imaging, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Bounce Imaging
provider_slug: bounce-imaging
slug: bounce-imaging-domain-security
source_filename: bounce-imaging-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bounceimaging.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 11:17:01 2026 GMT\n  hsts: null\ndomains:\n- domain: bounceimaging.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bounce-imaging/refs/heads/main/security/bounce-imaging-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Imaging
- Law Enforcement
- Defense
- Public Safety
---
