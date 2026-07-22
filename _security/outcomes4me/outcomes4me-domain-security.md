---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: outcomes4me.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: outcomes4me.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outcomes4Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outcomes4Me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Outcomes4Me
provider_slug: outcomes4me
slug: outcomes4me-domain-security
source_filename: outcomes4me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outcomes4me.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: outcomes4me.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outcomes4me/refs/heads/main/security/outcomes4me-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Digital Health
- Healthcare
- Cancer
- Oncology
- Patient Engagement
- Real-world Data
- Clinical Trials
---
