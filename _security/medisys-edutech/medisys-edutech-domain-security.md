---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: smarteach.com
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: app.smarteach.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Medisys Edutech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MediSys EduTech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MediSys EduTech
provider_slug: medisys-edutech
slug: medisys-edutech-domain-security
source_filename: medisys-edutech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.smarteach.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: smarteach.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/medisys-edutech/security/medisys-edutech-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Education
- Healthcare
- E‑learning
- DigitalHealth
---
