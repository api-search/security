---
api_specs:
- filename: monte-carlo-graph-ql-api-openapi.yml
  format: yaml
  label: Monte Carlo Graph QL API
  slug: monte-carlo-graph-ql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monte-carlo/refs/heads/main/openapi/monte-carlo-graph-ql-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: montecarlo.ai
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 iodef "mailto:domains@montecarlodata.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getmontecarlo.com
  spf: true
hosts:
- cert_expires: Nov 14 02:18:58 2026 GMT
  host: montecarlo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 14:48:10 2026 GMT
  host: docs.getmontecarlo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: api.getmontecarlo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Monte Carlo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monte Carlo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Monte Carlo
provider_slug: monte-carlo
slug: monte-carlo-domain-security
source_filename: monte-carlo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: montecarlo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 02:18:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.getmontecarlo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 14:48:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getmontecarlo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: montecarlo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getmontecarlo.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 iodef \"mailto:domains@montecarlodata.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monte-carlo/refs/heads/main/security/monte-carlo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Observability
- Data Quality
- Data Reliability
- Data Lake
- Data Warehouse
- Lineage
- Monitoring
- AI Observability
---
