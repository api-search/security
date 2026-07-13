---
api_specs:
- filename: docusign-openapi-original.yml
  format: yaml
  label: Docusign eSignature REST API
  slug: docusign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-openapi-original.yml
- filename: docusign-admin-openapi-original.yml
  format: yaml
  label: Docusign Admin API
  slug: docusign-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-admin-openapi-original.yml
- filename: docusign-click-openapi-original.yml
  format: yaml
  label: Docusign Click API
  slug: docusign-click-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-click-openapi-original.yml
- filename: docusign-maestro-openapi-original.yml
  format: yaml
  label: Docusign Maestro API
  slug: docusign-maestro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-maestro-openapi-original.yml
- filename: docusign-monitor-openapi-original.yml
  format: yaml
  label: Docusign Monitor API
  slug: docusign-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-monitor-openapi-original.yml
- filename: docusign-rooms-openapi-original.yml
  format: yaml
  label: Docusign Rooms API
  slug: docusign-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/openapi/docusign-rooms-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: docusign.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:traffic@docusign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: docusign.net
  spf: true
hosts:
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: developers.docusign.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: demo.docusign.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: api-d.docusign.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docusign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docusign, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Docusign
provider_slug: docusign
slug: docusign-domain-security
source_filename: docusign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.docusign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: demo.docusign.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-d.docusign.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: docusign.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: docusign.net\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:traffic@docusign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/security/docusign-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
---
