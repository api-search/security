---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: affymedtech.com
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: affymedtech.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Affy Medtech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Affy MedTech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Affy MedTech
provider_slug: affy-medtech
slug: affy-medtech-domain-security
source_filename: affy-medtech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: affymedtech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: affymedtech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affy-medtech/refs/heads/main/security/affy-medtech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Care
- Health IT
- Electronic Health Records
- openEHR
- Hospital Management
- Medical Records
- Interoperability
- Remote Diagnostics
- United Kingdom
---
