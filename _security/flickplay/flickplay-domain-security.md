---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flickplay.co
  spf: true
hosts:
- cert_expires: Sep 23 22:33:21 2026 GMT
  host: www.flickplay.co
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flickplay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flickplay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flickplay
provider_slug: flickplay
slug: flickplay-domain-security
source_filename: flickplay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flickplay.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:33:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: flickplay.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flickplay/refs/heads/main/security/flickplay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Web3
- Gaming
- Social
- Augmented Reality
- Consumer Apps
- Character IP
- Entertainment
---
