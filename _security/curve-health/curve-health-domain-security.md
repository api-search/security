---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: curvehealth.com
  spf: false
hosts:
- cert_expires: Oct  7 03:05:57 2026 GMT
  host: www.curvehealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Curve Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curve Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Curve Health
provider_slug: curve-health
slug: curve-health-domain-security
source_filename: curve-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.curvehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:05:57 2026 GMT\n  hsts: false\ndomains:\n- domain: curvehealth.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curve-health/refs/heads/main/security/curve-health-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Health
- Healthcare
- Telemedicine
- Telehealth
- Digital Health
- Senior Care
- Skilled Nursing
- Health Information Exchange
- Predictive Analytics
---
