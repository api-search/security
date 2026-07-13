---
api_specs:
- filename: superlinked-openapi.yml
  format: yaml
  label: Superlinked Ingestion API
  slug: superlinked-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superlinked/refs/heads/main/openapi/superlinked-openapi.yml
- filename: superlinked-openapi.yml
  format: yaml
  label: Superlinked Query API
  slug: superlinked-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superlinked/refs/heads/main/openapi/superlinked-openapi.yml
- filename: superlinked-openapi.yml
  format: yaml
  label: Superlinked Data Loader API
  slug: superlinked-data-loader-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superlinked/refs/heads/main/openapi/superlinked-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:infrastructure-staff@python.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: pypi.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: superlinked.com
  spf: false
hosts:
- cert_expires: Jan 29 04:33:07 2027 GMT
  host: pypi.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 11:35:05 2026 GMT
  host: www.superlinked.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superlinked Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superlinked, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Superlinked
provider_slug: superlinked
slug: superlinked-domain-security
source_filename: superlinked-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pypi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 04:33:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.superlinked.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 11:35:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pypi.org\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:infrastructure-staff@python.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: superlinked.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superlinked/refs/heads/main/security/superlinked-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Vectors
- Embeddings
- Vector Search
- Retrieval
- Recommendations
- RAG
---
