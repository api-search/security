---
api_specs:
- filename: knotch-events-api-openapi.yml
  format: yaml
  label: Knotch Events API
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knotch/refs/heads/main/openapi/knotch-events-api-openapi.yml
- filename: knotch-health-api-openapi.yml
  format: yaml
  label: Knotch Health API
  slug: knotch-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knotch/refs/heads/main/openapi/knotch-health-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: knotch.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: knotch.it
  spf: true
hosts:
- cert_expires: Nov 11 12:51:48 2026 GMT
  host: knotch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: knotch.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 04:32:29 2026 GMT
  host: help.knotch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knotch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knotch, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Knotch
provider_slug: knotch
slug: knotch-domain-security
source_filename: knotch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knotch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 12:51:48 2026 GMT\n  hsts: false\n- host: knotch.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.knotch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 04:32:29 2026 GMT\n  hsts: false\ndomains:\n- domain: knotch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: knotch.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knotch/refs/heads/main/security/knotch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Content Intelligence
- Content Marketing
- Analytics
- Artificial Intelligence
- Personalization
- Marketing Technology
- Agentic Web
- Conversion Tracking
- Attribution
- Event Ingestion
- Web Analytics
---
