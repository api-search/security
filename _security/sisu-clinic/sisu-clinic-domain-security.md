---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sisuclinic.com
  spf: true
hosts:
- cert_expires: Aug 20 08:11:49 2026 GMT
  host: www.sisuclinic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sisu Clinic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sisu Clinic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sisu Clinic
provider_slug: sisu-clinic
slug: sisu-clinic-domain-security
source_filename: sisu-clinic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sisuclinic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 08:11:49 2026 GMT\n  hsts: null\ndomains:\n- domain: sisuclinic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sisu-clinic/refs/heads/main/security/sisu-clinic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Medical Aesthetics
- Cosmetic Medicine
- Aesthetics
- Clinic
- Consumer Health
---
