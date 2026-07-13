---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cheetaho.com
  spf: true
hosts:
- cert_expires: Sep  1 06:01:51 2026 GMT
  host: cheetaho.com
  hsts: true
  hsts_max_age: 768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cheetaho Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CheetahO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CheetahO
provider_slug: cheetaho
slug: cheetaho-domain-security
source_filename: cheetaho-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cheetaho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 06:01:51 2026 GMT\n  hsts: true\n  hsts_max_age: 768000\ndomains:\n- domain: cheetaho.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cheetaho/refs/heads/main/security/cheetaho-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Photography
- Public APIs
---
