---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vanti-analytics.com
  spf: false
hosts:
- cert_expires: Sep 30 23:06:45 2026 GMT
  host: www.vanti-analytics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vanti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vanti Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Vanti Analytics
provider_slug: vanti
slug: vanti-domain-security
source_filename: vanti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  The vanti-analytics.com domain has lapsed and is no longer operated by\n  Vanti Analytics (www serves a FASTPANEL parked page; the apex redirects to\n  an unrelated site). These probe results describe the current squatter\n  hosting, not company-operated infrastructure.\nhosts:\n- host: www.vanti-analytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:06:45 2026 GMT\n  hsts: false\ndomains:\n- domain: vanti-analytics.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vanti/refs/heads/main/security/vanti-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Manufacturing
- Machine Learning
- Predictive Quality
- Defect Detection
- Industrial
---
