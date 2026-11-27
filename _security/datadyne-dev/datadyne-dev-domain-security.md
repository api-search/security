---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: datadyne.dev
  spf: true
hosts:
- cert_expires: Dec  5 07:07:14 2026 GMT
  host: datadyne.dev
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DataDyne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataDyne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: DataDyne
provider_slug: datadyne-dev
slug: datadyne-dev-domain-security
source_filename: datadyne-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datadyne.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 07:07:14 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: datadyne.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/datadyne-dev/security/datadyne-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- automotive repair
- KPI dashboard
- Shop Management
- Multi-Location
---
