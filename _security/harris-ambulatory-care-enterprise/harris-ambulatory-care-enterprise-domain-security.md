---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: harrisambulatory.com
  spf: true
hosts:
- cert_expires: Sep 15 04:51:46 2026 GMT
  host: harrisambulatory.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harris Ambulatory Care Enterprise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harris Ambulatory Care Enterprise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Harris Ambulatory Care Enterprise
provider_slug: harris-ambulatory-care-enterprise
slug: harris-ambulatory-care-enterprise-domain-security
source_filename: harris-ambulatory-care-enterprise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: harrisambulatory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:51:46 2026 GMT\n  hsts: false\ndomains:\n- domain: harrisambulatory.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harris-ambulatory-care-enterprise/refs/heads/main/security/harris-ambulatory-care-enterprise-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Ambulatory Care
- Electronic Health Records
- FHIR
- Health IT
- Healthcare
- ONC Certified
- Pulse
---
