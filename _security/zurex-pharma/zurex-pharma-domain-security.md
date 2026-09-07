---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zurexpharma.com
  spf: true
hosts:
- cert_expires: Nov 10 12:17:41 2026 GMT
  host: www.zurexpharma.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zurex Pharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zurex Pharma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zurex Pharma
provider_slug: zurex-pharma
slug: zurex-pharma-domain-security
source_filename: zurex-pharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zurexpharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 12:17:41 2026 GMT\n  hsts: null\ndomains:\n- domain: zurexpharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zurex-pharma/refs/heads/main/security/zurex-pharma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Pharmaceuticals
- Medical Devices
- Healthcare
- Antimicrobials
- Infection Prevention
- Life Sciences
- Wisconsin
---
