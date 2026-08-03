---
api_specs:
- filename: pryon-admin-openapi.json
  format: json
  label: Pryon Admin API
  slug: pryon-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/openapi/pryon-admin-openapi.json
- filename: pryon-retrieval-may2025-openapi.json
  format: json
  label: Pryon Retrieval API
  slug: pryon-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/openapi/pryon-retrieval-may2025-openapi.json
- filename: pryon-generative-openapi.json
  format: json
  label: Pryon Generative API
  slug: pryon-generative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/openapi/pryon-generative-openapi.json
- filename: pryon-knowledge-collections-may2025-openapi.json
  format: json
  label: Pryon Knowledge Collections API
  slug: pryon-knowledge-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/openapi/pryon-knowledge-collections-may2025-openapi.json
- filename: pryon-exchange-may2025-openapi.json
  format: json
  label: Pryon Exchange API
  slug: pryon-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/openapi/pryon-exchange-may2025-openapi.json
- filename: pryon-feedback-august2025-openapi.json
  format: json
  label: Pryon Feedback API
  slug: pryon-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/openapi/pryon-feedback-august2025-openapi.json
- filename: pryon-universal-connector-may2025-openapi.json
  format: json
  label: Pryon Universal Connector API
  slug: pryon-universal-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/openapi/pryon-universal-connector-may2025-openapi.json
- filename: pryon-user-defined-metadata-may2025-openapi.json
  format: json
  label: Pryon User-Defined Metadata API
  slug: pryon-user-defined-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/openapi/pryon-user-defined-metadata-may2025-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pryon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pryon.net
  spf: true
hosts:
- cert_expires: Oct 12 10:20:04 2026 GMT
  host: www.pryon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 21:46:40 2026 GMT
  host: docs.pryon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 20:44:50 2026 GMT
  host: api.pryon.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pryon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pryon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Pryon
provider_slug: pryon
slug: pryon-domain-security
source_filename: pryon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pryon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 10:20:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pryon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:46:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pryon.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:44:50 2026 GMT\n  hsts: null\ndomains:\n- domain: pryon.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pryon.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pryon/refs/heads/main/security/pryon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Retrieval Augmented Generation
- Enterprise Search
- Knowledge Management
- Generative AI
- Document Ingestion
- Content Connectors
- Agents
- Machine Learning
- Company
---
