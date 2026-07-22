---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:HOSTMASTER@hanover.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hanover.com
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: www.hanover.com
  hsts: true
  hsts_max_age: 3000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hanover Insurance Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hanover Insurance Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hanover Insurance Group
provider_slug: hanover-insurance-group
slug: hanover-insurance-group-domain-security
source_filename: hanover-insurance-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hanover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 3000\ndomains:\n- domain: hanover.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:HOSTMASTER@hanover.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hanover-insurance-group/refs/heads/main/security/hanover-insurance-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Property and Casualty
- Financial Services
- Fortune 500
---
