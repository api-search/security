---
api_specs:
- filename: metabase-openapi.yml
  format: yaml
  label: Metabase API
  slug: metabase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabase/refs/heads/main/openapi/metabase-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: metabase.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: your-metabase-instance.com
  spf: false
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: www.metabase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: your-metabase-instance.com
  https: false
kind: domain-security
layout: security
method: probed
name: Metabase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metabase, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Metabase
provider_slug: metabase
slug: metabase-domain-security
source_filename: metabase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.metabase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: your-metabase-instance.com\n  https: false\ndomains:\n- domain: metabase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: your-metabase-instance.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metabase/refs/heads/main/security/metabase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Open Source
- SQL
---
