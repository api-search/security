---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thirtymadison.com
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: thirtymadison.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thirty Madison Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thirty Madison, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Thirty Madison
provider_slug: thirty-madison
slug: thirty-madison-domain-security
source_filename: thirty-madison-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thirtymadison.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: thirtymadison.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thirty-madison/refs/heads/main/security/thirty-madison-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Telehealth
- Telemedicine
- Digital Health
- Direct-to-Consumer
- Pharmacy
---
