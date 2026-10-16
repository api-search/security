---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ki.se
  spf: true
hosts:
- cert_expires: Nov 17 14:49:59 2026 GMT
  host: ki.se
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Karolinska Institutet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Karolinska Institutet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Karolinska Institutet
provider_slug: karolinska-institutet
slug: karolinska-institutet-domain-security
source_filename: karolinska-institutet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ki.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 14:49:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ki.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karolinska-institutet/refs/heads/main/security/karolinska-institutet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Education
- Research
- Healthcare
- Sweden
---
