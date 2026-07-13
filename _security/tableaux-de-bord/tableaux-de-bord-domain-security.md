---
api_specs:
- filename: grafana-dashboard-openapi.yml
  format: yaml
  label: Grafana HTTP API
  slug: grafana
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableaux-de-bord/refs/heads/main/openapi/grafana-dashboard-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: grafana.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: your-grafana-instance.com
  spf: false
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: grafana.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: your-grafana-instance.com
  https: false
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: www.metabase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tableaux De Bord Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tableaux De Bord, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tableaux De Bord
provider_slug: tableaux-de-bord
slug: tableaux-de-bord-domain-security
source_filename: tableaux-de-bord-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grafana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: your-grafana-instance.com\n  https: false\n- host: www.metabase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: grafana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: your-grafana-instance.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tableaux-de-bord/refs/heads/main/security/tableaux-de-bord-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Dashboards
- Business Intelligence
- Analytics
- Data Visualization
- Monitoring
- Grafana
- Metabase
---
