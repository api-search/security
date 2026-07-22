---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: keepface.com
  spf: true
hosts:
- cert_expires: Aug 21 18:23:27 2026 GMT
  host: keepface.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keepface Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KeepFace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: KeepFace
provider_slug: keepface
slug: keepface-domain-security
source_filename: keepface-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keepface.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 18:23:27 2026 GMT\n  hsts: null\ndomains:\n- domain: keepface.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keepface/refs/heads/main/security/keepface-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Influencer Marketing
- Creator Economy
- Marketing
- Social Media
- Affiliate Marketing
- Advocacy
- Campaign Management
---
