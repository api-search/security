---
api_specs:
- filename: infisical-infisical-api-openapi.yml
  format: yaml
  label: Infisical REST API
  slug: infisical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infisical/refs/heads/main/openapi/infisical-infisical-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: infisical.com
  spf: true
hosts:
- cert_expires: Sep 22 17:03:05 2026 GMT
  host: infisical.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: app.infisical.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: us.infisical.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infisical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infisical, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Infisical
provider_slug: infisical
slug: infisical-domain-security
source_filename: infisical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infisical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 17:03:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.infisical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us.infisical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: infisical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infisical/refs/heads/main/security/infisical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Secrets Management
- Security
- DevOps
- Developer Tools
- Open Source
- PKI
- Certificates
- Privileged Access Management
- CI/CD
- Kubernetes
- Environment Variables
- Encryption
---
