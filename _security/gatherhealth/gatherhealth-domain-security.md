---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gatherhealth.com
  spf: true
hosts:
- cert_expires: Sep 21 00:40:29 2026 GMT
  host: www.gatherhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gatherhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gatherhealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Gatherhealth
provider_slug: gatherhealth
slug: gatherhealth-domain-security
source_filename: gatherhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gatherhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:40:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gatherhealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gatherhealth/refs/heads/main/security/gatherhealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Healthcare
- Primary Care
- Senior Care
- Medicare
- Value-Based Care
- Health Services
---
