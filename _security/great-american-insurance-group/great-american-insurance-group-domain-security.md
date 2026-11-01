---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gaig.com
  spf: true
hosts:
- cert_expires: Mar 23 23:59:59 2027 GMT
  host: gaig.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Great American Insurance Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Great American Insurance Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Great American Insurance Group
provider_slug: great-american-insurance-group
slug: great-american-insurance-group-domain-security
source_filename: great-american-insurance-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gaig.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gaig.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/great-american-insurance-group/security/great-american-insurance-group-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Insurance
- Property
- Casualty
- Specialty
- Financial-Services
- Company
---
