---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dayamedikapratama.com
  spf: true
hosts:
- cert_expires: Oct 11 10:33:32 2026 GMT
  host: dayamedikapratama.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Daya Medika Pratama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daya Medika Pratama, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Daya Medika Pratama
provider_slug: daya-medika-pratama
slug: daya-medika-pratama-domain-security
source_filename: daya-medika-pratama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dayamedikapratama.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 10:33:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dayamedikapratama.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daya-medika-pratama/refs/heads/main/security/daya-medika-pratama-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Health Information System
- Electronic Health Records
- openEHR
- FHIR
- Hospital
- Insurance
- Systems Integrator
- Microsoft Dynamics 365
- Indonesia
---
