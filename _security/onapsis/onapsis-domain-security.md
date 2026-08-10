---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: onapsis.com
  spf: true
hosts:
- cert_expires: Oct 15 13:30:15 2026 GMT
  host: onapsis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onapsis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onapsis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Onapsis
provider_slug: onapsis
slug: onapsis-domain-security
source_filename: onapsis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onapsis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 13:30:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: onapsis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onapsis/refs/heads/main/security/onapsis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Application Security
- Vulnerability Management
- Compliance
- SAP
- ERP
- Threat Detection
- GraphQL
- Enterprise Software
---
