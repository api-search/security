---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kychospitality.com
  spf: true
hosts:
- cert_expires: Dec 12 07:58:48 2026 GMT
  host: kychospitality.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kyc Hospitality Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KYC Hospitality, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: KYC Hospitality
provider_slug: kyc-hospitality
slug: kyc-hospitality-domain-security
source_filename: kyc-hospitality-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kychospitality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 07:58:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kychospitality.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kyc-hospitality/security/kyc-hospitality-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hospitality
- Compliance
- IdentityVerification
- SaaS
---
