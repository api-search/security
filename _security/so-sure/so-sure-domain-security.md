---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: wearesosure.com
  spf: true
hosts:
- cert_expires: Oct 15 01:23:54 2026 GMT
  host: wearesosure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: So Sure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for So Sure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: So Sure
provider_slug: so-sure
slug: so-sure-domain-security
source_filename: so-sure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wearesosure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 01:23:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wearesosure.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/so-sure/refs/heads/main/security/so-sure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Insurance
- InsurTech
- Mobile Insurance
- Contents Insurance
- Consumer
- United Kingdom
---
