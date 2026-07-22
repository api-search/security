---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fronterahealth.com
  spf: false
hosts:
- cert_expires: Oct 13 23:06:17 2026 GMT
  host: fronterahealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Frontera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frontera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Frontera
provider_slug: frontera
slug: frontera-domain-security
source_filename: frontera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fronterahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:06:17 2026 GMT\n  hsts: false\ndomains:\n- domain: fronterahealth.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frontera/refs/heads/main/security/frontera-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Behavioral Health
- Artificial Intelligence
- Clinical Documentation
- ABA Therapy
- Autism Care
- HIPAA
---
