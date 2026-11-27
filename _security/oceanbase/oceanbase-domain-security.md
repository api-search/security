---
api_specs:
- filename: oceanbase-openapi-generated.yml
  format: yaml
  label: OceanBase API
  slug: oceanbase-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oceanbase/openapi/_ae-authored/oceanbase-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oceanbase.com
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: oceanbase.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OceanBase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OceanBase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OceanBase
provider_slug: oceanbase
slug: oceanbase-domain-security
source_filename: oceanbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oceanbase.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: oceanbase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/oceanbase/security/oceanbase-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Distributed Database
- Cloud Database
- Open Source Database
- AI Native Search
- Real-Time Analytics
- Mission-Critical Transactions
---
