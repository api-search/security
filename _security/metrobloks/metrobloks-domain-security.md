---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: metrobloks.com
  spf: true
hosts:
- cert_expires: Oct  4 22:32:49 2026 GMT
  host: metrobloks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metrobloks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metrobloks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Metrobloks
provider_slug: metrobloks
slug: metrobloks-domain-security
source_filename: metrobloks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metrobloks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:32:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: metrobloks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metrobloks/refs/heads/main/security/metrobloks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Centers
- Colocation
- Interconnection
- Edge Computing
- AI Infrastructure
- Digital Infrastructure
- Cloud Infrastructure
- Low Latency
- Liquid Cooling
- Sustainability
- Commercial Real Estate
- United States
- France
---
