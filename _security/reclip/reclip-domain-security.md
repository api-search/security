---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reclip.app
  spf: true
hosts:
- cert_expires: Jan  4 02:50:40 2027 GMT
  host: reclip.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Reclip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reclip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reclip
provider_slug: reclip
slug: reclip-domain-security
source_filename: reclip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reclip.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 02:50:40 2027 GMT\n  hsts: false\ndomains:\n- domain: reclip.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reclip/refs/heads/main/security/reclip-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Social
- Mobile
- PhotoSharing
- VideoSharing
- Real-Time
---
