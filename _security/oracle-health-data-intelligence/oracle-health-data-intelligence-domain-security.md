---
api_specs:
- filename: oracle-health-data-intelligence-openapi.yml
  format: yaml
  label: Oracle Health Data Intelligence
  slug: oracle-health-data-intelligence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-health-data-intelligence/refs/heads/main/openapi/oracle-health-data-intelligence-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: healtheintent.com
  spf: false
hosts:
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: docs.healtheintent.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: cernerdemo.api.us-1.healtheintent.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oracle Health Data Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Health Data Intelligence, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Oracle Health Data Intelligence
provider_slug: oracle-health-data-intelligence
slug: oracle-health-data-intelligence-domain-security
source_filename: oracle-health-data-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.healtheintent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: false\n- host: cernerdemo.api.us-1.healtheintent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: healtheintent.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-health-data-intelligence/refs/heads/main/security/oracle-health-data-intelligence-domain-security.yml
summary_line: TLSv1.3
tags:
- Genomic
- Health Records
- Healthcare
---
