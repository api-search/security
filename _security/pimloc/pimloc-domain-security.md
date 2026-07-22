---
api_specs:
- filename: secureredact-openapi.yml
  format: yaml
  label: Secure Redact API
  slug: secure-redact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pimloc/refs/heads/main/openapi/secureredact-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: secureredact.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: secureredact.co.uk
  spf: true
hosts:
- cert_expires: Sep 19 06:17:43 2026 GMT
  host: www.secureredact.ai
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 20:08:35 2026 GMT
  host: app.secureredact.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pimloc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pimloc, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pimloc
provider_slug: pimloc
slug: pimloc-domain-security
source_filename: pimloc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.secureredact.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 06:17:43 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: app.secureredact.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 20:08:35 2026 GMT\n  hsts: false\ndomains:\n- domain: secureredact.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: secureredact.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pimloc/refs/heads/main/security/pimloc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Privacy
- Video Redaction
- Anonymization
- PII
- Data Protection
- Artificial Intelligence
- Compliance
- Video Analytics
---
