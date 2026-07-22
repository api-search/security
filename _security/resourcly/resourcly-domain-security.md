---
api_specs:
- filename: resourcly-openapi-original.json
  format: json
  label: Resourcly API
  slug: resourcly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resourcly/refs/heads/main/openapi/resourcly-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: resourcly.com
  spf: true
hosts:
- cert_expires: Oct 12 21:24:45 2026 GMT
  host: resourcly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 21:24:45 2026 GMT
  host: api.resourcly.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Resourcly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resourcly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Resourcly
provider_slug: resourcly
slug: resourcly-domain-security
source_filename: resourcly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: resourcly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 21:24:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.resourcly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 21:24:45 2026 GMT\n  hsts: null\ndomains:\n- domain: resourcly.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resourcly/refs/heads/main/security/resourcly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Manufacturing
- Inventory Optimization
- PLM
- ERP
- Procurement
- Supply Chain
- Artificial Intelligence
- Data Harmonization
- Similarity Search
- BOM
---
