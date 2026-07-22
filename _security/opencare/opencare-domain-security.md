---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opencare.com
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: opencare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opencare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opencare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Opencare
provider_slug: opencare
slug: opencare-domain-security
source_filename: opencare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opencare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: opencare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opencare/refs/heads/main/security/opencare-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Dental
- Healthcare
- Marketplace
- Appointments
- Booking
- Consumer
- Reviews
---
