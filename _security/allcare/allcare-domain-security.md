---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: allcare.ph
  spf: true
hosts:
- cert_expires: Jan 14 06:43:02 2027 GMT
  host: allcare.ph
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AllCare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AllCare
provider_slug: allcare
slug: allcare-domain-security
source_filename: allcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: allcare.ph\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 06:43:02 2027 GMT\n  hsts: null\ndomains:\n- domain: allcare.ph\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allcare/refs/heads/main/security/allcare-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Insurance
- Employee Benefits
- HMO
- Teleconsultation
- Insurtech
- Philippines
- SME
---
