---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: anteoshealth.com
  spf: true
hosts:
- cert_expires: Jan 24 02:06:46 2027 GMT
  host: anteoshealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anteos Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anteos Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Anteos Health
provider_slug: anteoshealth-com
slug: anteoshealth-com-domain-security
source_filename: anteoshealth-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anteoshealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 02:06:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anteoshealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/anteoshealth-com/security/anteoshealth-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- Artificial Intelligence
- Medical Software
- Telehealth
- France
---
