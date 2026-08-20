---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: doctoranywhere.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: doctoranywhere.co.th
  spf: false
hosts:
- cert_expires: Oct 12 21:18:55 2026 GMT
  host: doctoranywhere.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:58:53 2026 GMT
  host: doctoranywhere.co.th
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 06:05:10 2026 GMT
  host: www.doctoranywhere.my
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doctor Anywhere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Doctor Anywhere, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Doctor Anywhere
provider_slug: doctor-anywhere
slug: doctor-anywhere-domain-security
source_filename: doctor-anywhere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doctoranywhere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 21:18:55 2026 GMT\n  hsts: null\n- host: doctoranywhere.co.th\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:58:53 2026 GMT\n  hsts: null\n- host: www.doctoranywhere.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 06:05:10 2026 GMT\n  hsts: null\ndomains:\n- domain: doctoranywhere.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: doctoranywhere.co.th\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doctor-anywhere/refs/heads/main/security/doctor-anywhere-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Telehealth
- Telemedicine
- Digital Health
- Health Screening
- Corporate Wellness
- Singapore
- Southeast Asia
- MCP
---
