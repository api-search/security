---
api_specs:
- filename: appen-download-api-openapi.yml
  format: yaml
  label: Appen Download API
  slug: appen-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-download-api-openapi.yml
- filename: appen-internal-contributors-api-openapi.yml
  format: yaml
  label: Appen Internal Contributors API
  slug: appen-internal-contributors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-internal-contributors-api-openapi.yml
- filename: appen-jobs-api-openapi.yml
  format: yaml
  label: Appen Jobs API
  slug: appen-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-jobs-api-openapi.yml
- filename: appen-projects-api-openapi.yml
  format: yaml
  label: Appen Projects API
  slug: appen-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-projects-api-openapi.yml
- filename: appen-route-units-api-openapi.yml
  format: yaml
  label: Appen Route Units API
  slug: appen-route-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-route-units-api-openapi.yml
- filename: appen-test-questions-api-openapi.yml
  format: yaml
  label: Appen Test Questions API
  slug: appen-test-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-test-questions-api-openapi.yml
- filename: appen-upload-api-openapi.yml
  format: yaml
  label: Appen Upload API
  slug: appen-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-upload-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.appen.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appen.com
  spf: true
hosts:
- cert_expires: Dec  5 01:30:32 2026 GMT
  host: appen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Appen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Appen
provider_slug: appen
slug: appen-domain-security
source_filename: appen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 01:30:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: appen.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.appen.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/security/appen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Data
- Annotation
- Training Data
- Enterprise
---
