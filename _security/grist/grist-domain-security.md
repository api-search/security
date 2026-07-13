---
api_specs:
- filename: grist.yml
  format: yaml
  label: Grist REST API
  slug: grist-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/gristlabs/grist-help/master/api/grist.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getgrist.com
  spf: true
hosts:
- cert_expires: Oct  7 08:51:50 2026 GMT
  host: www.getgrist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 14:16:48 2026 GMT
  host: support.getgrist.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: docs.getgrist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grist, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Grist
provider_slug: grist
slug: grist-domain-security
source_filename: grist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getgrist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 08:51:50 2026 GMT\n  hsts: false\n- host: support.getgrist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:16:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: docs.getgrist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: getgrist.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/security/grist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Spreadsheet
- Database
- Collaboration
- No-Code
- Data Management
- Webhooks
- Open Source
---
