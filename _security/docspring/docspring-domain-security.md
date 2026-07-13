---
api_specs:
- filename: openapi.json
  format: json
  label: DocSpring API
  slug: docspring-api
  spec_type: OpenAPI
  url: https://docspring.com/api-docs/v1/openapi.json
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: docspring.com
  spf: true
hosts:
- cert_expires: Oct  4 22:46:48 2026 GMT
  host: docspring.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 08:03:26 2026 GMT
  host: sync.api.docspring.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docspring Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DocSpring, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DocSpring
provider_slug: docspring
slug: docspring-domain-security
source_filename: docspring-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docspring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:46:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sync.api.docspring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 08:03:26 2026 GMT\n  hsts: null\ndomains:\n- domain: docspring.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docspring/refs/heads/main/security/docspring-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- PDF
- Document Generation
- PDF Templates
- E-Signatures
- Forms
- HTML to PDF
- Document Automation
---
