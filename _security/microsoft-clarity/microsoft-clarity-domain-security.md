---
api_specs:
- filename: microsoft-clarity-openapi.yml
  format: yaml
  label: Microsoft Clarity API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-clarity/refs/heads/main/openapi/microsoft-clarity-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clarity.ms
  spf: false
hosts:
- cert_expires: Oct 27 17:31:24 2026 GMT
  host: clarity.microsoft.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 14:15:13 2026 GMT
  host: www.clarity.ms
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Microsoft Clarity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Clarity, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Clarity
provider_slug: microsoft-clarity
slug: microsoft-clarity-domain-security
source_filename: microsoft-clarity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clarity.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 17:31:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.clarity.ms\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 29 14:15:13 2026 GMT\n  hsts: false\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: clarity.ms\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-clarity/refs/heads/main/security/microsoft-clarity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Heatmaps
- Session Recording
- Web Analytics
---
