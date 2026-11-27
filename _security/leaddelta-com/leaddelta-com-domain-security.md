---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: leaddelta.com
  spf: true
hosts:
- cert_expires: Jan 22 19:01:30 2027 GMT
  host: leaddelta.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LeadDelta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeadDelta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LeadDelta
provider_slug: leaddelta-com
slug: leaddelta-com-domain-security
source_filename: leaddelta-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leaddelta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 19:01:30 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: leaddelta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/leaddelta-com/security/leaddelta-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- LinkedIn
- Artificial Intelligence
- Sales
- Collaboration
---
