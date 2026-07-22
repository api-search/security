---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: playtika.com
  spf: true
hosts:
- cert_expires: Aug 30 00:15:45 2026 GMT
  host: www.playtika.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Playtika Holding Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Playtika Holding, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Playtika Holding
provider_slug: playtika-holding
slug: playtika-holding-domain-security
source_filename: playtika-holding-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.playtika.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 00:15:45 2026 GMT\n  hsts: false\ndomains:\n- domain: playtika.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playtika-holding/refs/heads/main/security/playtika-holding-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Gaming
- Mobile Games
- Entertainment
---
