---
api_specs:
- filename: mendix-apps-api-openapi.yml
  format: yaml
  label: Mendix Apps API
  slug: mendix-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendix/refs/heads/main/openapi/mendix-apps-api-openapi.yml
- filename: mendix-environments-api-openapi.yml
  format: yaml
  label: Mendix Environments API
  slug: mendix-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendix/refs/heads/main/openapi/mendix-environments-api-openapi.yml
- filename: mendix-logs-api-openapi.yml
  format: yaml
  label: Mendix Logs API
  slug: mendix-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendix/refs/heads/main/openapi/mendix-logs-api-openapi.yml
- filename: mendix-packages-api-openapi.yml
  format: yaml
  label: Mendix Packages API
  slug: mendix-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendix/refs/heads/main/openapi/mendix-packages-api-openapi.yml
- filename: mendix-tags-api-openapi.yml
  format: yaml
  label: Mendix Tags API
  slug: mendix-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendix/refs/heads/main/openapi/mendix-tags-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog ; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 iodef "mailto:security@mendix.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mendix.com
  spf: true
hosts:
- cert_expires: Nov 27 17:11:33 2026 GMT
  host: www.mendix.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: docs.mendix.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: deploy.mendix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Mendix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mendix, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mendix
provider_slug: mendix
slug: mendix-domain-security
source_filename: mendix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mendix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 17:11:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.mendix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: deploy.mendix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mendix.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog ; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 iodef \"mailto:security@mendix.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mendix/refs/heads/main/security/mendix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Low-Code
- Application Development
- Enterprise Platform
- Application Lifecycle
- Deployment
- Governance
---
