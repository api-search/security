---
api_specs:
- filename: koala-io-openapi.yml
  format: yaml
  label: Koala Collection (Batch) API
  slug: koala-io-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/openapi/koala-io-openapi.yml
- filename: koala-io-openapi.yml
  format: yaml
  label: Koala Accounts API
  slug: koala-io-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/openapi/koala-io-openapi.yml
- filename: koala-io-openapi.yml
  format: yaml
  label: Koala SDK Bootstrap API
  slug: koala-io-sdk-bootstrap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/openapi/koala-io-openapi.yml
- filename: koala-io-openapi.yml
  format: yaml
  label: Koala Deletion (GDPR) API
  slug: koala-io-deletion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/openapi/koala-io-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getkoala.com
  spf: true
hosts:
- cert_expires: Sep 15 16:00:11 2026 GMT
  host: getkoala.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 23:43:14 2026 GMT
  host: app.getkoala.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 23:43:14 2026 GMT
  host: api2.getkoala.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Koala Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koala, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Koala
provider_slug: koala-io
slug: koala-io-domain-security
source_filename: koala-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getkoala.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:00:11 2026 GMT\n  hsts: false\n- host: app.getkoala.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:43:14 2026 GMT\n  hsts: null\n- host: api2.getkoala.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:43:14 2026 GMT\n  hsts: null\ndomains:\n- domain: getkoala.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/security/koala-io-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Buyer Intent
- Visitor Identification
- De-anonymization
- Enrichment
- Go-to-Market
- Sales Intelligence
- B2B
---
