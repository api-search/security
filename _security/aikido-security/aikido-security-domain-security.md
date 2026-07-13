---
api_specs:
- filename: getopenapispec
  format: yaml
  label: Aikido Security REST API
  slug: aikido-rest-api
  spec_type: OpenAPI
  url: https://apidocs.aikido.dev/reference/getopenapispec
description: ''
domains:
- caa:
  - 0 iodef "mailto:support@aikido.dev"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aikido.dev
  spf: true
hosts:
- cert_expires: Oct  1 15:24:09 2026 GMT
  host: www.aikido.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 08:59:35 2026 GMT
  host: apidocs.aikido.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: app.aikido.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aikido Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aikido Security, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Aikido Security
provider_slug: aikido-security
slug: aikido-security-domain-security
source_filename: aikido-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aikido.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 15:24:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.aikido.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 08:59:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.aikido.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aikido.dev\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:support@aikido.dev\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aikido-security/refs/heads/main/security/aikido-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Pentesting
- API Security
- Application Security
- Cloud Security
- Compliance
- DAST
- Developer-First
- IaC Scanning
- SAST
- SCA
- Secret Detection
---
