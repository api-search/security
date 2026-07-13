---
api_specs:
- filename: parseur-openapi.yml
  format: yaml
  label: Parseur API
  slug: parseur-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parseur/refs/heads/main/openapi/parseur-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: parseur.com
  spf: true
hosts:
- cert_expires: Sep 15 00:49:32 2026 GMT
  host: parseur.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 14:33:07 2026 GMT
  host: app.parseur.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 21 00:05:23 2026 GMT
  host: developer.parseur.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Parseur Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parseur, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Parseur
provider_slug: parseur
slug: parseur-domain-security
source_filename: parseur-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parseur.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 00:49:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.parseur.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:33:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.parseur.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 21 00:05:23 2026 GMT\n  hsts: false\ndomains:\n- domain: parseur.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parseur/refs/heads/main/security/parseur-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Artificial Intelligence
- Document Parsing
- Document Processing
- Document Extraction
- Email Parsing
- OCR
- Data Extraction
- Vision AI
- Automation
- Webhooks
- Mailboxes
- SaaS
---
