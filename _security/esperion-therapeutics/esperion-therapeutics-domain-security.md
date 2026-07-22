---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: esperion.com
  spf: true
hosts:
- cert_expires: Aug  7 09:27:36 2026 GMT
  host: www.esperion.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Esperion Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Esperion Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Esperion Therapeutics
provider_slug: esperion-therapeutics
slug: esperion-therapeutics-domain-security
source_filename: esperion-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.esperion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 09:27:36 2026 GMT\n  hsts: null\ndomains:\n- domain: esperion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esperion-therapeutics/refs/heads/main/security/esperion-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Pharmaceutical
- Biotechnology
- Life Sciences
- Cardiovascular
- Healthcare
- Therapeutics
---
