---
api_specs:
- filename: string-db-annotation-api-openapi.yml
  format: yaml
  label: STRING Annotation API
  slug: string-db-annotation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/string-db/refs/heads/main/openapi/string-db-annotation-api-openapi.yml
- filename: string-db-enrichment-api-openapi.yml
  format: yaml
  label: STRING Enrichment API
  slug: string-db-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/string-db/refs/heads/main/openapi/string-db-enrichment-api-openapi.yml
- filename: string-db-homology-api-openapi.yml
  format: yaml
  label: STRING Homology API
  slug: string-db-homology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/string-db/refs/heads/main/openapi/string-db-homology-api-openapi.yml
- filename: string-db-identifiers-api-openapi.yml
  format: yaml
  label: STRING Identifiers API
  slug: string-db-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/string-db/refs/heads/main/openapi/string-db-identifiers-api-openapi.yml
- filename: string-db-network-api-openapi.yml
  format: yaml
  label: STRING Network API
  slug: string-db-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/string-db/refs/heads/main/openapi/string-db-network-api-openapi.yml
- filename: string-db-utility-api-openapi.yml
  format: yaml
  label: STRING Utility API
  slug: string-db-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/string-db/refs/heads/main/openapi/string-db-utility-api-openapi.yml
- filename: string-db-valuesranks-api-openapi.yml
  format: yaml
  label: STRING Valuesranks API
  slug: string-db-valuesranks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/string-db/refs/heads/main/openapi/string-db-valuesranks-api-openapi.yml
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
