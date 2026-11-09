---
api_specs:
- filename: dirigon-com-openapi-generated.yml
  format: yaml
  label: Dirigon API
  slug: dirigon-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dirigon-com/openapi/_ae-authored/dirigon-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dirigon.com
  spf: true
hosts:
- cert_expires: Jan  7 10:27:37 2027 GMT
  host: dirigon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dirigon Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dirigon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dirigon
provider_slug: dirigon-com
slug: dirigon-com-domain-security
source_filename: dirigon-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dirigon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 10:27:37 2027 GMT\n  hsts: false\ndomains:\n- domain: dirigon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dirigon-com/security/dirigon-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Credit
- Data
- SEC
---
