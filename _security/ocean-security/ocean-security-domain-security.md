---
api_specs:
- filename: ocean-security-openapi.yml
  format: yaml
  label: Ocean Security API
  slug: ocean-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-security/refs/heads/main/openapi/ocean-security-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "pki.goog"
  - 0 issue "starfieldtech.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ocean.security
  spf: true
hosts:
- cert_expires: Aug 23 20:32:26 2026 GMT
  host: ocean.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 05:11:29 2026 GMT
  host: docs.ocean.security
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 01:18:32 2026 GMT
  host: api.ocean.security
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ocean Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ocean Security, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ocean Security
provider_slug: ocean-security
slug: ocean-security-domain-security
source_filename: ocean-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ocean.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 20:32:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ocean.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 05:11:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ocean.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 01:18:32 2026 GMT\n  hsts: null\ndomains:\n- domain: ocean.security\n  dnssec: true\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"starfieldtech.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocean-security/refs/heads/main/security/ocean-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Email Security
- Cybersecurity
- Phishing
- Threat Detection
- Email
- Anti-Phishing
- Artificial Intelligence
- Threat Intelligence
---
