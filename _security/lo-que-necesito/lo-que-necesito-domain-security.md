---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: loquenecesito.co
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: loquenecesito.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lo Que Necesito Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lo Que Necesito, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lo Que Necesito
provider_slug: lo-que-necesito
slug: lo-que-necesito-domain-security
source_filename: lo-que-necesito-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loquenecesito.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: loquenecesito.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lo-que-necesito/refs/heads/main/security/lo-que-necesito-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- PropTech
- Housing
- Colombia
- Latin America
---
