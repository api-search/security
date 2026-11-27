---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: syntheticuserlab.space
  spf: false
hosts:
- cert_expires: Feb  4 18:07:48 2027 GMT
  host: syntheticuserlab.space
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SyntheticUser Lab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SyntheticUser Lab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SyntheticUser Lab
provider_slug: syntheticuserlab-space
slug: syntheticuserlab-space-domain-security
source_filename: syntheticuserlab-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: syntheticuserlab.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 18:07:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: syntheticuserlab.space\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/syntheticuserlab-space/security/syntheticuserlab-space-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- UserTesting
- Prototyping
- SaaS
- Synthetic Personas
- Company
---
