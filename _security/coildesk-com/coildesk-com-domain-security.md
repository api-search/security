---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coildesk.com
  spf: true
hosts:
- cert_expires: Jan 20 12:59:11 2027 GMT
  host: coildesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coildesk Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for coildesk-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: coildesk-com
provider_slug: coildesk-com
slug: coildesk-com-domain-security
source_filename: coildesk-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coildesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 12:59:11 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coildesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/coildesk-com/security/coildesk-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HVAC
- Contractor
- Software
- Tools
- WorkOrder
- Pricing
- Invoicing
---
