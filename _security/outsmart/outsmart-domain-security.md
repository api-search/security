---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: joinoutsmart.com
  spf: true
hosts:
- cert_expires: Aug 25 00:59:29 2026 GMT
  host: joinoutsmart.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outsmart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outsmart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Outsmart
provider_slug: outsmart
slug: outsmart-domain-security
source_filename: outsmart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joinoutsmart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 00:59:29 2026 GMT\n  hsts: false\ndomains:\n- domain: joinoutsmart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outsmart/refs/heads/main/security/outsmart-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- EdTech
- Higher Education
- Mobile
- Consumer
- Learning
---
