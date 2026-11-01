---
api_specs:
- filename: tropia-pl-openapi.yml
  format: yaml
  label: tropia.pl API
  slug: tropia-pl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tropia-pl/openapi/tropia-pl-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tropia.pl
  spf: true
hosts:
- cert_expires: Dec 18 13:14:36 2026 GMT
  host: tropia.pl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tropia Pl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tropia-pl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: tropia-pl
provider_slug: tropia-pl
slug: tropia-pl-domain-security
source_filename: tropia-pl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tropia.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 13:14:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tropia.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/tropia-pl/security/tropia-pl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API
- Data
- Poland
- Finance
- Public-Records
---
