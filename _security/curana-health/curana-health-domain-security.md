---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: curanahealth.com
  spf: true
hosts:
- cert_expires: Sep 15 06:48:57 2026 GMT
  host: curanahealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 17:21:25 2026 GMT
  host: fhir.curanahealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Curana Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curana Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Curana Health
provider_slug: curana-health
slug: curana-health-domain-security
source_filename: curana-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curanahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 06:48:57 2026 GMT\n  hsts: false\n- host: fhir.curanahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 17:21:25 2026 GMT\n  hsts: null\ndomains:\n- domain: curanahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curana-health/refs/heads/main/security/curana-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Digital Health
- Healthcare
- FHIR
- Interoperability
- Medicare Advantage
- Senior Living
- Patient Access
- Value-Based Care
- CMS-9115-F
---
