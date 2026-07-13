---
api_specs:
- filename: dolthub-openapi.yml
  format: yaml
  label: DoltHub SQL Query API
  slug: dolthub-sql-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolthub/refs/heads/main/openapi/dolthub-openapi.yml
- filename: dolthub-openapi.yml
  format: yaml
  label: DoltHub Write API
  slug: dolthub-write-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolthub/refs/heads/main/openapi/dolthub-openapi.yml
- filename: dolthub-openapi.yml
  format: yaml
  label: DoltHub Repositories and Branches API
  slug: dolthub-repositories-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dolthub/refs/heads/main/openapi/dolthub-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dolthub.com
  spf: true
hosts:
- cert_expires: Sep 20 21:50:23 2026 GMT
  host: www.dolthub.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 21:50:23 2026 GMT
  host: docs.dolthub.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dolthub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DoltHub, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DoltHub
provider_slug: dolthub
slug: dolthub-domain-security
source_filename: dolthub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dolthub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 21:50:23 2026 GMT\n  hsts: false\n- host: docs.dolthub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 21:50:23 2026 GMT\n  hsts: false\ndomains:\n- domain: dolthub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dolthub/refs/heads/main/security/dolthub-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Database
- SQL
- Version Control
- Git for Data
- MySQL
---
