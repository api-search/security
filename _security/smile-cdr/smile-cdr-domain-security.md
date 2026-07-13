---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smiledigitalhealth.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smilecdr.com
  spf: true
hosts:
- cert_expires: Oct  4 06:14:37 2026 GMT
  host: www.smiledigitalhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 05:31:23 2026 GMT
  host: smilecdr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Smile Cdr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smile Digital Health, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Smile Digital Health
provider_slug: smile-cdr
slug: smile-cdr-domain-security
source_filename: smile-cdr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smiledigitalhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 06:14:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: smilecdr.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 05:31:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: smiledigitalhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: smilecdr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smile-cdr/refs/heads/main/security/smile-cdr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- FHIR
- HL7
- Clinical Data Repository
- Interoperability
- HAPI FHIR
- SMART on FHIR
- Terminology Services
- MDM
- Bulk Data
- Subscriptions
- CMS Interoperability
- Prior Authorization
- Digital Quality Measures
- CQL
- Payer
- Provider
- Health Information Exchange
---
