---
api_specs:
- filename: cybrary-completions-api-openapi.yml
  format: yaml
  label: Cybrary Completions API
  slug: cybrary-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybrary/refs/heads/main/openapi/cybrary-completions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cybrary.it
  spf: true
hosts:
- cert_expires: Oct 15 15:21:19 2026 GMT
  host: www.cybrary.it
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 01:56:04 2026 GMT
  host: help.cybrary.it
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: app.cybrary.it
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cybrary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cybrary, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cybrary
provider_slug: cybrary
slug: cybrary-domain-security
source_filename: cybrary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cybrary.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 15:21:19 2026 GMT\n  hsts: null\n- host: help.cybrary.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 01:56:04 2026 GMT\n  hsts: null\n- host: app.cybrary.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cybrary.it\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cybrary/refs/heads/main/security/cybrary-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cybersecurity
- Training
- Education
- Learning Management
- Certification
- Workforce Development
- xAPI
- SCIM
- Security Awareness
---
