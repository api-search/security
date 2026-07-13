---
api_specs:
- filename: rest
  format: yaml
  label: Google Looker Studio API
  slug: google-looker-studio-api
  spec_type: OpenAPI
  url: https://lookerstudio.googleapis.com/$discovery/rest
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: datastudio.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Looker Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Looker Studio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Looker Studio
provider_slug: google-looker-studio
slug: google-looker-studio-domain-security
source_filename: google-looker-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datastudio.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-looker-studio/refs/heads/main/security/google-looker-studio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Google
- Looker
- Reporting
---
