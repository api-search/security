---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jains.com
  spf: true
hosts:
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: www.jains.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jains Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jain Irrigation Systems Ltd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jain Irrigation Systems Ltd
provider_slug: jains
slug: jains-domain-security
source_filename: jains-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jains.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: jains.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jains/refs/heads/main/security/jains-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Agriculture
- Irrigation
- Micro Irrigation
- Drip Irrigation
- Piping
- Plastics
- Solar Energy
- Tissue Culture
- Food Processing
- Manufacturing
- India
- AgTech
---
