---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: serviceup.com
  spf: true
hosts:
- cert_expires: Sep 10 18:16:32 2026 GMT
  host: www.serviceup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 17:34:13 2026 GMT
  host: api.serviceup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Serviceup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ServiceUp, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ServiceUp
provider_slug: serviceup
slug: serviceup-domain-security
source_filename: serviceup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.serviceup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 18:16:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.serviceup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 17:34:13 2026 GMT\n  hsts: null\ndomains:\n- domain: serviceup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serviceup/refs/heads/main/security/serviceup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fleet Management
- Vehicle Repair
- Automotive
- Insurance
- Maintenance
- Agentic AI
- Model Context Protocol
- Transportation
---
