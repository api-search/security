---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: emaillistvalidation.com
  spf: true
hosts:
- cert_expires: Feb  4 20:05:05 2027 GMT
  host: emaillistvalidation.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Email List Validation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Email List Validation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Email List Validation
provider_slug: emaillistvalidation-com
slug: emaillistvalidation-com-domain-security
source_filename: emaillistvalidation-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emaillistvalidation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 20:05:05 2027 GMT\n  hsts: false\ndomains:\n- domain: emaillistvalidation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/emaillistvalidation-com/security/emaillistvalidation-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email Verification
- Data Cleaning
- API Service
- Marketing Tools
- Software-as-a-Service
---
