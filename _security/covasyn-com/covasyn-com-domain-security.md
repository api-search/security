---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: covasyn.com
  spf: true
hosts:
- cert_expires: Jan 27 09:01:34 2027 GMT
  host: covasyn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CovaSyn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CovaSyn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CovaSyn
provider_slug: covasyn-com
slug: covasyn-com-domain-security
source_filename: covasyn-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: covasyn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 09:01:34 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: covasyn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/covasyn-com/security/covasyn-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Chemistry
- Pharma
- Biotechnology
- Cheminformatics
- MCP
- Artificial Intelligence
- Quality and Regulatory
---
