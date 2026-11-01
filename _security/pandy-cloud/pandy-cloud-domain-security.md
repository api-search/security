---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pandy.cloud
  spf: true
hosts:
- cert_expires: Dec 27 05:44:40 2026 GMT
  host: pandy.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pandy Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pandy-cloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: pandy-cloud
provider_slug: pandy-cloud
slug: pandy-cloud-domain-security
source_filename: pandy-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pandy.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 05:44:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pandy.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/pandy-cloud/security/pandy-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CRM
- ERP
- Scheduling
- SaaS
---
