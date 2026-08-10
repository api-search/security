---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: steno.com
  spf: true
hosts:
- cert_expires: Aug 24 10:33:43 2026 GMT
  host: steno.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 11:18:08 2026 GMT
  host: help.steno.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 10:33:43 2026 GMT
  host: api.steno.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  note: 'automated probe first recorded hsts null; re-probed by hand three times (curl -I and curl -X HEAD) and the header is present on the 403 response as strict-transport-security: max-age=31557600'
  tls_version: TLSv1.3
- host: brief.steno.com
  hsts: true
  hsts_max_age: 31536000
  https: true
- host: status.steno.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
- host: trust.steno.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
kind: domain-security
layout: security
method: probed
name: Steno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Steno, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 6 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Steno
provider_slug: steno
slug: steno-domain-security
source_filename: steno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: steno.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 10:33:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: help.steno.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 11:18:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.steno.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 10:33:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n  note: 'automated probe first recorded hsts null; re-probed by hand three times (curl\n    -I and curl -X HEAD) and the header is present on the 403 response as strict-transport-security:\n    max-age=31557600'\n- host: brief.steno.com\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n- host: status.steno.com\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: trust.steno.com\n\
  \  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\ndomains:\n- domain: steno.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nx-evidence:\n  fetched: '2026-08-05'\n  tool: 0-working/probe-domain-security.py, plus a manual curl re-probe of api.steno.com\n    and the three subdomains the script did not carry\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steno/refs/heads/main/security/steno-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Legal
- Legal Technology
- Court Reporting
- Depositions
- Litigation Support
- Transcription
- Video
- Artificial Intelligence
- Salesforce
---
