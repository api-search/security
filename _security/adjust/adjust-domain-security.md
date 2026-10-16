---
api_specs:
- filename: adjust-openapi-generated.yml
  format: yaml
  label: Adjust API
  slug: adjust-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adjust/refs/heads/main/openapi/_ae-authored/adjust-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adjust.com
  spf: true
hosts:
- cert_expires: Dec 19 01:00:08 2026 GMT
  host: www.adjust.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adjust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adjust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Adjust
provider_slug: adjust
slug: adjust-domain-security
source_filename: adjust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adjust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 01:00:08 2026 GMT\n  hsts: null\ndomains:\n- domain: adjust.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adjust/refs/heads/main/security/adjust-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Measurement
- Analytics
- Attribution
- Deep Linking
- Fraud Prevention
- Mobile Marketing
- AI Solutions
- Gaming
---
