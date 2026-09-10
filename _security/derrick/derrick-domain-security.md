---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: derrick-app.com
  spf: true
hosts:
- cert_expires: Nov  1 17:34:13 2026 GMT
  host: app1.derrick-app.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 17:34:13 2026 GMT
  host: derrick-app.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Derrick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Derrick, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Derrick
provider_slug: derrick
slug: derrick-domain-security
source_filename: derrick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app1.derrick-app.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 17:34:13 2026 GMT\n  hsts: null\n- host: derrick-app.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 17:34:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: derrick-app.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/derrick/refs/heads/main/security/derrick-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- b2b-data-enrichment
- email-finder
- phone-finder
- company-firmographics
- lead-generation
- sales-intelligence
- crm-enrichment
- tech-stack-detection
- email-verification
- siret-siren-france
- mcp-server
- llms-txt
- google-sheets
- gtm-tools
---
