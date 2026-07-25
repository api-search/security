---
api_specs:
- filename: microsoft-defender-alerts-api-openapi.yml
  format: yaml
  label: Microsoft Defender Alerts API
  slug: microsoft-defender-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-defender/refs/heads/main/openapi/microsoft-defender-alerts-api-openapi.yml
- filename: microsoft-defender-machines-api-openapi.yml
  format: yaml
  label: Microsoft Defender Machines API
  slug: microsoft-defender-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-defender/refs/heads/main/openapi/microsoft-defender-machines-api-openapi.yml
- filename: microsoft-defender-vulnerabilities-api-openapi.yml
  format: yaml
  label: Microsoft Defender Vulnerabilities API
  slug: microsoft-defender-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-defender/refs/heads/main/openapi/microsoft-defender-vulnerabilities-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Nov  6 23:03:08 2026 GMT
  host: security.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 11:56:27 2026 GMT
  host: api.security.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 09:09:00 2026 GMT
  host: us.api.security.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Defender Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Defender, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Defender
provider_slug: microsoft-defender
slug: microsoft-defender-domain-security
source_filename: microsoft-defender-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: security.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:03:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.security.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 11:56:27 2026 GMT\n  hsts: null\n- host: us.api.security.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 09:09:00 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-defender/refs/heads/main/security/microsoft-defender-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
