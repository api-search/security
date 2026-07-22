---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aquashieldai.com
  spf: true
hosts:
- cert_expires: Sep 11 02:44:21 2026 GMT
  host: aquashieldai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aquashield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AquaShield, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AquaShield
provider_slug: aquashield
slug: aquashield-domain-security
source_filename: aquashield-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aquashieldai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 02:44:21 2026 GMT\n  hsts: null\ndomains:\n- domain: aquashieldai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aquashield/refs/heads/main/security/aquashield-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Water
- Leak Detection
- IoT
- Sensors
- Real Estate
- PropTech
- Artificial Intelligence
- Y Combinator
---
