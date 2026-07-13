---
api_specs:
- filename: llms.txt
  format: yaml
  label: PostGrid Print & Mail API
  slug: print-mail-api
  spec_type: OpenAPI
  url: https://postgrid.readme.io/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: postgrid.com
  spf: true
hosts:
- cert_expires: Sep 15 07:00:50 2026 GMT
  host: www.postgrid.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 07:00:50 2026 GMT
  host: docs.postgrid.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 07:00:50 2026 GMT
  host: api.postgrid.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Postgrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PostGrid, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PostGrid
provider_slug: postgrid
slug: postgrid-domain-security
source_filename: postgrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.postgrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:00:50 2026 GMT\n  hsts: false\n- host: docs.postgrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:00:50 2026 GMT\n  hsts: null\n- host: api.postgrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:00:50 2026 GMT\n  hsts: null\ndomains:\n- domain: postgrid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postgrid/refs/heads/main/security/postgrid-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Direct Mail
- Print & Mail
- Address Verification
- Address Validation
- Postcards
- Letters
- Checks
- Physical Mail
- Mail Automation
- Address Autocomplete
- Geocoding
---
