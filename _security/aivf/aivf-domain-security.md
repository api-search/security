---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aivf.co
  spf: true
hosts:
- cert_expires: Sep  4 01:34:58 2026 GMT
  host: www.aivf.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aivf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AiVF, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AiVF
provider_slug: aivf
slug: aivf-domain-security
source_filename: aivf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aivf.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 01:34:58 2026 GMT\n  hsts: false\ndomains:\n- domain: aivf.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aivf/refs/heads/main/security/aivf-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Fertility
- IVF
- Artificial Intelligence
- Medical Devices
- Embryology
- Reproductive Health
---
