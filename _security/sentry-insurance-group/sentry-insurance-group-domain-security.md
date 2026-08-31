---
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  - 128 issue "awstrust.com"
  - 128 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sentry.com
  spf: true
hosts:
- cert_expires: Nov  2 14:24:22 2026 GMT
  host: www.sentry.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sentry Insurance Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sentry Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sentry Insurance
provider_slug: sentry-insurance-group
slug: sentry-insurance-group-domain-security
source_filename: sentry-insurance-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sentry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 14:24:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sentry.com\n  dnssec: false\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"awstrust.com\"\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentry-insurance-group/refs/heads/main/security/sentry-insurance-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 1000
- Insurance
- Property and Casualty Insurance
- Commercial Insurance
- Workers Compensation
- Auto Insurance
- Retirement
- Annuities
- Mutual Insurance
- Financial-Services
- Trucking
- Wisconsin
- United States
---
