---
api_specs:
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore CDN API
  slug: cdn
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore Cloud API
  slug: cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore Object Storage API
  slug: storage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore DNS API
  slug: dns
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore Streaming API
  slug: streaming
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore Everywhere Inference API
  slug: inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore Security & WAAP API
  slug: security-waap
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore FastEdge API
  slug: fastedge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com "
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "admins@gcore.lu"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gcore.com
  spf: true
hosts:
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: gcore.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: api.gcore.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gcore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gcore, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gcore
provider_slug: gcore
slug: gcore-domain-security
source_filename: gcore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gcore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: false\n- host: api.gcore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gcore.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com \"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"admins@gcore.lu\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/security/gcore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Edge Cloud
- CDN
- Streaming
- Edge AI
- Infrastructure
---
