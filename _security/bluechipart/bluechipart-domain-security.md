---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bluechipart.co
  spf: true
hosts:
- cert_expires: Dec 16 20:12:38 2026 GMT
  host: bluechipart.co
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bluechipart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bluechipart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bluechipart
provider_slug: bluechipart
slug: bluechipart-domain-security
source_filename: bluechipart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bluechipart.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 20:12:38 2026 GMT\n  hsts: true\n  hsts_max_age: 16000000\ndomains:\n- domain: bluechipart.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluechipart/refs/heads/main/security/bluechipart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Art
- ArtDealer
- BlueChipArt
- Secondary Market
- Collectors
---
