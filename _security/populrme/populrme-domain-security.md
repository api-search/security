---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: populr.me
  spf: true
hosts:
- cert_expires: Sep 25 17:24:44 2026 GMT
  host: populr.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Populrme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Populr.me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Populr.me
provider_slug: populrme
slug: populrme-domain-security
source_filename: populrme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: populr.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:24:44 2026 GMT\n  hsts: null\ndomains:\n- domain: populr.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/populrme/refs/heads/main/security/populrme-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Website Builder
- Web Publishing
- Landing Pages
- Content Management
- Defunct
---
