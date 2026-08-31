---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: petfolk.com
  spf: true
hosts:
- cert_expires: Oct 26 04:31:50 2026 GMT
  host: petfolk.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Petfolk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Petfolk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Petfolk
provider_slug: petfolk
slug: petfolk-domain-security
source_filename: petfolk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: petfolk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 04:31:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: petfolk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/petfolk/refs/heads/main/security/petfolk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- veterinary
- veterinary-care
- animal-health
- pet-care
- pet-health
- healthcare
- telehealth
- virtual-care
- urgent-care
- clinics
- membership
- consumer-health
- mobile-app
- north-carolina
---
