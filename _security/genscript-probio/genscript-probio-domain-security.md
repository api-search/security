---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: probiocdmo.com
  spf: true
hosts:
- cert_expires: Nov 16 13:32:33 2026 GMT
  host: www.probiocdmo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Genscript Probio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genscript Probio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Genscript Probio
provider_slug: genscript-probio
slug: genscript-probio-domain-security
source_filename: genscript-probio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.probiocdmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 13:32:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: probiocdmo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genscript-probio/refs/heads/main/security/genscript-probio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Pharmaceuticals
- Contract Manufacturing
- CDMO
- Cell and Gene Therapy
- Biologics
- Manufacturing
---
