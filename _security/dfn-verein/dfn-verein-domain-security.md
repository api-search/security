---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dfn.de
  spf: true
hosts:
- cert_expires: Apr 17 13:09:34 2027 GMT
  host: www.dfn.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dfn Verein Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DFN-Verein, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: DFN-Verein
provider_slug: dfn-verein
slug: dfn-verein-domain-security
source_filename: dfn-verein-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dfn.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 17 13:09:34 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dfn.de\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dfn-verein/refs/heads/main/security/dfn-verein-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Research
- Education
- Networking
- Security
- Cloud
---
