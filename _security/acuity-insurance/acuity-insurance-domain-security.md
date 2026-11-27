---
description: ''
domains:
- caa:
  - 128 issue "globalsign.com"
  - 128 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acuity.com
  spf: true
hosts:
- cert_expires: Jan 15 18:01:20 2027 GMT
  host: acuity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Acuity Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acuity Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Acuity Insurance
provider_slug: acuity-insurance
slug: acuity-insurance-domain-security
source_filename: acuity-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acuity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 18:01:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: acuity.com\n  dnssec: false\n  caa:\n  - 128 issue \"globalsign.com\"\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/acuity-insurance/security/acuity-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Mutual
- Personal Insurance
- Business Insurance
---
