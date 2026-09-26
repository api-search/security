---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: andieswim.com
  spf: true
hosts:
- cert_expires: Oct 27 16:52:01 2026 GMT
  host: andieswim.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Andie Swim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Andie Swim, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Andie Swim
provider_slug: andie-swim
slug: andie-swim-domain-security
source_filename: andie-swim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: andieswim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 16:52:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: andieswim.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andie-swim/refs/heads/main/security/andie-swim-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Swimwear
- Fashion
- E-commerce
- InclusiveSizing
- Lifestyle
---
