---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agenceelan.ca
  spf: true
hosts:
- cert_expires: Jan 26 22:00:14 2027 GMT
  host: agenceelan.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Élan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Élan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Élan
provider_slug: agenceelan-ca
slug: agenceelan-ca-domain-security
source_filename: agenceelan-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agenceelan.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 22:00:14 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agenceelan.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agenceelan-ca/security/agenceelan-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Custom Software
- Quebec
- Software-as-a-Service
- Automation
- Company
---
