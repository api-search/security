---
description: ''
domains:
- caa:
  - 0 issuemail "amazon.com"
  - 0 issuemail "digicert.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: domo.com
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: www.domo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: developer.domo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.domo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Domo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Domo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Domo
provider_slug: domo
slug: domo-domain-security
source_filename: domo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.domo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: null\n- host: developer.domo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: null\n- host: api.domo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: domo.com\n  dnssec: false\n  caa:\n  - 0 issuemail \"amazon.com\"\n  - 0 issuemail \"digicert.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domo/refs/heads/main/security/domo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analysis
- Business Intelligence
- Data
- Pipelines
- Visualizations
---
