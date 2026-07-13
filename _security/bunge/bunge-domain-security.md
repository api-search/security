---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bunge.com
  spf: true
hosts:
- cert_expires: Sep 16 14:33:41 2026 GMT
  host: www.bunge.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bunge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bunge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bunge
provider_slug: bunge
slug: bunge-domain-security
source_filename: bunge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bunge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:33:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bunge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bunge/refs/heads/main/security/bunge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agribusiness
- Food
- Manufacturing
- Commodities
- Oilseeds
- Grain
- Biofuels
---
