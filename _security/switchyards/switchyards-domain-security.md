---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: switchyards.com
  spf: true
hosts:
- cert_expires: Oct 18 15:01:33 2026 GMT
  host: switchyards.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Switchyards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Switchyards, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Switchyards
provider_slug: switchyards
slug: switchyards-domain-security
source_filename: switchyards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: switchyards.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 15:01:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: switchyards.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/switchyards/refs/heads/main/security/switchyards-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Coworking
- Workspace
- Membership
- Productivity
- Coffee
---
