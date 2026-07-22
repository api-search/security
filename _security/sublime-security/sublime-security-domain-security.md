---
api_specs:
- filename: sublime-security-platform-openapi.json
  format: json
  label: Sublime Platform API
  slug: sublime-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-platform-openapi.json
- filename: sublime-security-multitenancy-openapi.json
  format: json
  label: Sublime Multi-Tenancy API (Beta)
  slug: sublime-multi-tenancy-api-beta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/openapi/sublime-security-multitenancy-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sublime.security
  spf: true
hosts:
- cert_expires: Oct 12 05:06:58 2026 GMT
  host: sublime.security
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sublime Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sublime Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sublime Security
provider_slug: sublime-security
slug: sublime-security-domain-security
source_filename: sublime-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sublime.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 05:06:58 2026 GMT\n  hsts: null\ndomains:\n- domain: sublime.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sublime-security/refs/heads/main/security/sublime-security-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Email Security
- Phishing
- Detection as Code
- Threat Detection
- Cloud Email Security
- SCIM
---
