---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: seafair.io
  spf: true
hosts:
- cert_expires: Aug 20 17:12:56 2026 GMT
  host: www.seafair.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seafair Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seafair, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Seafair
provider_slug: seafair
slug: seafair-domain-security
source_filename: seafair-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.seafair.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 17:12:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: seafair.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seafair/refs/heads/main/security/seafair-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Maritime
- Shipping
- ERP
- Compliance
- Crew Management
- Artificial Intelligence
---
