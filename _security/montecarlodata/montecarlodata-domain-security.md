---
api_specs:
- filename: apidocs.getmontecarlo.com
  format: yaml
  label: Monte Carlo GraphQL API
  slug: monte-carlo-graphql-api
  spec_type: OpenAPI
  url: https://apidocs.getmontecarlo.com
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: montecarlo.ai
  spf: true
- caa:
  - 0 issue "ssl.com"
  - 0 iodef "mailto:domains@montecarlodata.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getmontecarlo.com
  spf: true
hosts:
- cert_expires: Sep 15 21:09:01 2026 GMT
  host: montecarlo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 14:32:36 2026 GMT
  host: docs.getmontecarlo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: api.getmontecarlo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Montecarlodata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monte Carlo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Monte Carlo
provider_slug: montecarlodata
slug: montecarlodata-domain-security
source_filename: montecarlodata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: montecarlo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:09:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.getmontecarlo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:32:36 2026 GMT\n  hsts: null\n- host: api.getmontecarlo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: montecarlo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getmontecarlo.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 iodef \"mailto:domains@montecarlodata.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/montecarlodata/refs/heads/main/security/montecarlodata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Observability
- Data Quality
- Data Monitoring
- Data Lineage
- GraphQL
- AI Observability
- Data Reliability
---
