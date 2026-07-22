---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hiddendoor.co
  spf: true
hosts:
- cert_expires: Sep 17 16:43:56 2026 GMT
  host: www.hiddendoor.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hidden Door Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hidden Door, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hidden Door
provider_slug: hidden-door
slug: hidden-door-domain-security
source_filename: hidden-door-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hiddendoor.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:43:56 2026 GMT\n  hsts: false\ndomains:\n- domain: hiddendoor.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hidden-door/refs/heads/main/security/hidden-door-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Storytelling
- Interactive Fiction
- Roleplay
- Gaming
- Entertainment
- User Generated Content
---
