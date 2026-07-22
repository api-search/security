---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: seneca.systems
  spf: false
hosts:
- cert_expires: Aug 22 13:54:06 2026 GMT
  host: seneca.systems
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seneca Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seneca Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Seneca Systems
provider_slug: seneca-systems
slug: seneca-systems-domain-security
source_filename: seneca-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seneca.systems\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 13:54:06 2026 GMT\n  hsts: false\ndomains:\n- domain: seneca.systems\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seneca-systems/refs/heads/main/security/seneca-systems-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Govtech
- Government
- CRM
- Constituent Services
- Case Management
- Public Sector
- SaaS
---
