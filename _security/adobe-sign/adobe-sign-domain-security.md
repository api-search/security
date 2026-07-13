---
api_specs:
- filename: openapi
  format: yaml
  label: Adobe Acrobat Sign REST API
  slug: adobe-acrobat-sign-api
  spec_type: OpenAPI
  url: https://developer.adobe.com/acrobat-sign/docs/overview/sdks/openapi
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: adobesign.com
  spf: true
hosts:
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: www.adobe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 22:48:09 2026 GMT
  host: opensource.adobe.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: api.na4.adobesign.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adobe Sign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adobe Acrobat Sign, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adobe Acrobat Sign
provider_slug: adobe-sign
slug: adobe-sign-domain-security
source_filename: adobe-sign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adobe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\n- host: opensource.adobe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 20 22:48:09 2026 GMT\n  hsts: false\n- host: api.na4.adobesign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: adobesign.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-sign/refs/heads/main/security/adobe-sign-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Electronic Signature
- E-Signature
- Document Workflow
- Digital Signature
- Adobe
- Agreements
---
