---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: microhealth.com
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: microhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microhealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Microhealth
provider_slug: microhealth
slug: microhealth-domain-security
source_filename: microhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: microhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: microhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microhealth/refs/heads/main/security/microhealth-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Digital Health
- Healthcare
- Digital Therapeutics
- Hemophilia
- Bleeding Disorders
- Sickle Cell Disease
- Patient Engagement
- Real World Evidence
- Software as a Medical Device
---
