---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: contractors.fyi
  spf: true
hosts:
- cert_expires: Jan  4 21:50:26 2027 GMT
  host: contractors.fyi
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: contractors.fyi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for contractors.fyi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: contractors.fyi
provider_slug: contractors-fyi
slug: contractors-fyi-domain-security
source_filename: contractors-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contractors.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 21:50:26 2027 GMT\n  hsts: false\ndomains:\n- domain: contractors.fyi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/contractors-fyi/security/contractors-fyi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Contractors
- Home Improvement
- Building Permits
- Public Records
- MCP
- Real Estate
---
