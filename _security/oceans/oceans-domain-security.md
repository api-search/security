---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oceanshealthcare.com
  spf: true
hosts:
- cert_expires: Sep 26 06:03:27 2026 GMT
  host: oceanshealthcare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oceans Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oceans, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Oceans
provider_slug: oceans
slug: oceans-domain-security
source_filename: oceans-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oceanshealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 06:03:27 2026 GMT\n  hsts: false\ndomains:\n- domain: oceanshealthcare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oceans/refs/heads/main/security/oceans-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Behavioral Health
- Mental Health
- Psychiatric Hospitals
- Outpatient
- Telehealth
- Veterans Care
---
