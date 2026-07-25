---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tuvahealth.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: thetuvaproject.com
  spf: false
hosts:
- cert_expires: Sep 21 16:43:50 2026 GMT
  host: www.tuvahealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 16:15:28 2026 GMT
  host: thetuvaproject.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tuva Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tuva Health, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Tuva Health
provider_slug: tuva-health
slug: tuva-health-domain-security
source_filename: tuva-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tuvahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:43:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: thetuvaproject.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:15:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tuvahealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: thetuvaproject.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tuva-health/refs/heads/main/security/tuva-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- United States
- Health Data
- FHIR
- Interoperability
- Data Analytics
- Data Transformation
- Claims
- Open Source
- dbt
---
