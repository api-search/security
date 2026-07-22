---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rithmcap.com
  spf: true
hosts:
- cert_expires: Aug 31 23:59:59 2026 GMT
  host: www.rithmcap.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rithm Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rithm Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rithm Capital
provider_slug: rithm-capital
slug: rithm-capital-domain-security
source_filename: rithm-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rithmcap.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: rithmcap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rithm-capital/refs/heads/main/security/rithm-capital-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Alternative Asset Management
- Asset Management
- Financial Services
- Mortgage
- Real Estate
- REIT
---
