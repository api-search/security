---
api_specs:
- filename: threatconnect-openapi-generated.yml
  format: yaml
  label: ThreatConnect API
  slug: threatconnect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/openapi/_ae-authored/threatconnect-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: threatconnect.com
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: threatconnect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Threatconnect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThreatConnect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ThreatConnect
provider_slug: threatconnect
slug: threatconnect-domain-security
source_filename: threatconnect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: threatconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: threatconnect.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/threatconnect/refs/heads/main/security/threatconnect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Threat Intelligence
- Security Operations
- Platform
---
