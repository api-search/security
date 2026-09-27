---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lynq.io
  spf: true
hosts:
- cert_expires: Nov 13 00:50:41 2026 GMT
  host: lynq.io
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Awearableapparel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Awearableapparel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Awearableapparel
provider_slug: awearableapparel
slug: awearableapparel-domain-security
source_filename: awearableapparel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lynq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 00:50:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: lynq.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/awearableapparel/refs/heads/main/security/awearableapparel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Wearable
- Location
- IoT
- Safety
- Logistics
---
