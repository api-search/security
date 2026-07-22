---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: asktia.com
  spf: true
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: asktia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tia Women Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tia
provider_slug: tia-women
slug: tia-women-domain-security
source_filename: tia-women-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asktia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: asktia.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tia-women/refs/heads/main/security/tia-women-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Femtech
- Women's Health
- Primary Care
- Mental Health
- Gynecology
- Menopause
- Virtual Care
- Healthcare Clinics
- Membership
---
