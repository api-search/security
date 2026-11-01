---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ugc.fans
  spf: true
hosts:
- cert_expires: Jan  5 06:38:41 2027 GMT
  host: ugc.fans
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ugc Fans Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ugc-fans, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ugc-fans
provider_slug: ugc-fans
slug: ugc-fans-domain-security
source_filename: ugc-fans-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ugc.fans\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 06:38:41 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ugc.fans\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ugc-fans/security/ugc-fans-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- UGC
- ContentPlatform
- API
- Community
---
