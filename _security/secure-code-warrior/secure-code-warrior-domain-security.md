---
api_specs:
- filename: secure-code-warrior-portal-openapi.yml
  format: yaml
  label: Secure Code Warrior Portal API
  slug: secure-code-warrior-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/secure-code-warrior/refs/heads/main/openapi/secure-code-warrior-portal-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: securecodewarrior.com
  spf: true
hosts:
- cert_expires: Sep 10 18:43:30 2026 GMT
  host: www.securecodewarrior.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: portal-api.securecodewarrior.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:40:43 2026 GMT
  host: help.securecodewarrior.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Secure Code Warrior Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Secure Code Warrior, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Secure Code Warrior
provider_slug: secure-code-warrior
slug: secure-code-warrior-domain-security
source_filename: secure-code-warrior-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.securecodewarrior.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 18:43:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal-api.securecodewarrior.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.securecodewarrior.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:40:43 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: securecodewarrior.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/secure-code-warrior/refs/heads/main/security/secure-code-warrior-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Application Security
- Developer Training
- Security Education
- AppSec
- Secure Coding
- DevSecOps
---
