---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cult.fit
  spf: true
hosts:
- cert_expires: Dec 21 06:33:24 2026 GMT
  host: www.cult.fit
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Curefit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curefit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Curefit
provider_slug: curefit
slug: curefit-domain-security
source_filename: curefit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cult.fit\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 06:33:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cult.fit\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curefit/refs/heads/main/security/curefit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Fitness
- Wellness
- India
- Company
---
