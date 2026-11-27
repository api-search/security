---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: reelsfarm.com
  spf: true
hosts:
- cert_expires: Jan 16 03:43:03 2027 GMT
  host: reelsfarm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ReelsFarm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReelsFarm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ReelsFarm
provider_slug: reelsfarm-com
slug: reelsfarm-com-domain-security
source_filename: reelsfarm-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reelsfarm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 03:43:03 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reelsfarm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/reelsfarm-com/security/reelsfarm-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing Automation
- TikTok
- Instagram
- YouTube
- Facebook
---
