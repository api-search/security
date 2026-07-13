---
api_specs:
- filename: llms.txt
  format: yaml
  label: Inkit Document Generation API
  slug: inkit-document-generation-api
  spec_type: OpenAPI
  url: https://docs.inkit.com/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: inkit.com
  spf: true
hosts:
- cert_expires: Sep 10 03:16:15 2026 GMT
  host: www.inkit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:57:07 2026 GMT
  host: docs.inkit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 21:42:45 2026 GMT
  host: api.inkit.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inkit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inkit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Inkit
provider_slug: inkit
slug: inkit-domain-security
source_filename: inkit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inkit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 03:16:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.inkit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:57:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.inkit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 21:42:45 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: inkit.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inkit/refs/heads/main/security/inkit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Document Generation
- PDF
- Templates
- Digital Signatures
- Workflows
- Document Management
- Secure Documents
- Compliance
- HIPAA
- Enterprise
---
