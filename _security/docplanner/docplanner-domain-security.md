---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: docplanner.com
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.docplanner.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docplanner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docplanner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Docplanner
provider_slug: docplanner
slug: docplanner-domain-security
source_filename: docplanner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.docplanner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: docplanner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docplanner/refs/heads/main/security/docplanner-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- HealthTech
- Appointments
- Booking
- Medical
- SaaS
- Marketplace
- Doctors
- Telemedicine
---
