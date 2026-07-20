---
api_specs:
- filename: datto-rmm-openapi.json
  format: json
  label: Datto RMM API
  slug: datto-rmm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datto/refs/heads/main/openapi/datto-rmm-openapi.json
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "globalsign.com"
  - 0 issue "Digicert.com"
  - 0 issue "awstrust.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datto.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: centrastage.net
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: rmm.datto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: concord-api.centrastage.net
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Datto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datto, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Datto
provider_slug: datto
slug: datto-domain-security
source_filename: datto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rmm.datto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\n- host: concord-api.centrastage.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: datto.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"Digicert.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: centrastage.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datto/refs/heads/main/security/datto-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data Protection
- Backup
- Disaster Recovery
- Managed Service Providers
- Remote Monitoring and Management
- Endpoint Management
- Cybersecurity
- IT Operations
- SaaS Protection
---
