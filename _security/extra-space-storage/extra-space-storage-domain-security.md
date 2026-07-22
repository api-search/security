---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: extraspace.com
  spf: true
hosts:
- cert_expires: Sep 23 02:39:38 2026 GMT
  host: www.extraspace.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Extra Space Storage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Extra Space Storage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Extra Space Storage
provider_slug: extra-space-storage
slug: extra-space-storage-domain-security
source_filename: extra-space-storage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.extraspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 02:39:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: extraspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extra-space-storage/refs/heads/main/security/extra-space-storage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Self Storage
- Real Estate
- REIT
- Storage
---
