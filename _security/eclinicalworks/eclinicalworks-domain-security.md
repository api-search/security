---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eclinicalworks.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: healow.com
  spf: true
hosts:
- cert_expires: Sep 26 16:36:44 2026 GMT
  host: www.eclinicalworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: fhir.eclinicalworks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: connect4.healow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eclinicalworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eClinicalWorks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: eClinicalWorks
provider_slug: eclinicalworks
slug: eclinicalworks-domain-security
source_filename: eclinicalworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eclinicalworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:36:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fhir.eclinicalworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\n- host: connect4.healow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eclinicalworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: healow.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eclinicalworks/refs/heads/main/security/eclinicalworks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- EHR
- FHIR
- Healthcare
- Electronic Health Records
- Practice Management
- Clinical Data
- Health Information Exchange
- Patient Data
- Appointments
- Billing
- SMART on FHIR
---
