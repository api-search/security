---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: avidbots.com
  spf: true
hosts:
- cert_expires: Nov 29 17:35:45 2026 GMT
  host: avidbots.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avidbots Corp 9 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avidbots Corp., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Avidbots Corp.
provider_slug: avidbots-corp-9
slug: avidbots-corp-9-domain-security
source_filename: avidbots-corp-9-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avidbots.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 17:35:45 2026 GMT\n  hsts: false\ndomains:\n- domain: avidbots.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avidbots-corp-9/refs/heads/main/security/avidbots-corp-9-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Robotics
- Autonomous
- Cleaning
- Industrial
- Software-as-a-Service
---
