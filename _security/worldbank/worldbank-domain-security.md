---
api_specs:
- filename: v2
  format: yaml
  label: World Bank Indicators API
  slug: worldbank-indicators
  spec_type: OpenAPI
  url: https://api.worldbank.org/v2
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: worldbank.org
  spf: true
hosts:
- cert_expires: Aug 19 05:46:43 2026 GMT
  host: data.worldbank.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 11:29:58 2026 GMT
  host: datahelpdesk.worldbank.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 16:30:55 2026 GMT
  host: api.worldbank.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Worldbank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for World Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: World Bank
provider_slug: worldbank
slug: worldbank-domain-security
source_filename: worldbank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.worldbank.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 05:46:43 2026 GMT\n  hsts: false\n- host: datahelpdesk.worldbank.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:29:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.worldbank.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 16:30:55 2026 GMT\n  hsts: null\ndomains:\n- domain: worldbank.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldbank/refs/heads/main/security/worldbank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Development Data
- Global Economics
- GDP
- Poverty
- Health Metrics
- Education
- Climate
- Finance
- World Bank
- Open Data
- Country Data
- Indicators
---
