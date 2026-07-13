---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google AppSheet API
  slug: google-appsheet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-appsheet/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "pki.goog"
  - 0 issuewild "comodo.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: appsheet.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: support.google.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 09:10:06 2026 GMT
  host: api.appsheet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Appsheet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google AppSheet, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google AppSheet
provider_slug: google-appsheet
slug: google-appsheet-domain-security
source_filename: google-appsheet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: support.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: null\n- host: api.appsheet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 09:10:06 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: appsheet.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"comodo.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-appsheet/refs/heads/main/security/google-appsheet-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Applications
- Data
- Google
- Low-Code
- No-Code
- Tables
---
