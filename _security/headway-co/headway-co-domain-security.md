---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: headway.co
  spf: true
hosts:
- cert_expires: Aug 13 00:45:21 2026 GMT
  host: headway.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Headway Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Headway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Headway
provider_slug: headway-co
slug: headway-co-domain-security
source_filename: headway-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: headway.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 00:45:21 2026 GMT\n  hsts: null\ndomains:\n- domain: headway.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/headway-co/refs/heads/main/security/headway-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Mental Health
- Behavioral Health
- Therapy
- Psychiatry
- Telehealth
- Insurance
- Credentialing
- Claims
- Billing
- Practice Management
- EHR
- Provider Network
- Health Plans
- Healthtech
---
