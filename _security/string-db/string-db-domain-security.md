---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: STRING REST API
  slug: string-rest-api
  spec_type: OpenAPI
  url: https://string-db.org/help/api/
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: string-db.org
  spf: false
hosts:
- cert_expires: Aug 22 18:59:49 2026 GMT
  host: string-db.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: String Db Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for STRING, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: STRING
provider_slug: string-db
slug: string-db-domain-security
source_filename: string-db-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: string-db.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 18:59:49 2026 GMT\n  hsts: false\ndomains:\n- domain: string-db.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/string-db/refs/heads/main/security/string-db-domain-security.yml
summary_line: TLSv1.3
tags:
- Bioinformatics
- Proteins
- Genomics
- Life Sciences
- Research
- Open Data
---
