---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lovewick.com
  spf: true
hosts:
- cert_expires: Dec  6 01:04:10 2026 GMT
  host: lovewick.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lovewick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lovewick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lovewick
provider_slug: lovewick
slug: lovewick-domain-security
source_filename: lovewick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lovewick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 01:04:10 2026 GMT\n  hsts: false\ndomains:\n- domain: lovewick.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lovewick/refs/heads/main/security/lovewick-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Relationship
- App
- Couples
- Dating
- Wellness
---
