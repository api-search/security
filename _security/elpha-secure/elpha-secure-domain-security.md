---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elphasecure.com
  spf: true
hosts:
- cert_expires: Nov  8 18:36:36 2026 GMT
  host: www.elphasecure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: my.elphasecure.com
  hsts: false
  https: true
  note: Elpha Secure Portal (customer/broker sign-in). No Strict-Transport-Security response header observed.
  tls_version: TLSv1.3
- host: app.elphasecure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: help.elphasecure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: blog.elphasecure.com
  hsts: false
  https: true
  note: Ghost-hosted blog. No Strict-Transport-Security response header observed.
  tls_version: TLSv1.3
- host: trust.elphasecure.com
  http_status: 301
  https: true
  note: 'Resolves and answers, but redirects to itself (Location: https://trust.elphasecure.com) producing an infinite redirect loop; a bare GET without redirects returns 405. A trust-center subdomain appears provisioned but is not serving a document.'
  reachable: false
kind: domain-security
layout: security
method: probed
name: Elpha Secure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elpha Secure, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Elpha Secure
provider_slug: elpha-secure
slug: elpha-secure-domain-security
source_filename: elpha-secure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elphasecure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 18:36:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.elphasecure.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n  note: Elpha Secure Portal (customer/broker sign-in). No Strict-Transport-Security\n    response header observed.\n- host: app.elphasecure.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.elphasecure.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n- host: blog.elphasecure.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n  note: Ghost-hosted blog. No Strict-Transport-Security response header observed.\n- host: trust.elphasecure.com\n  https: true\n  reachable: false\n  http_status: 301\n  note: 'Resolves and answers, but redirects to itself (Location:\
  \ https://trust.elphasecure.com)\n    producing an infinite redirect loop; a bare GET without redirects returns 405.\n    A trust-center subdomain appears provisioned but is not serving a document.'\ndomains:\n- domain: elphasecure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elpha-secure/refs/heads/main/security/elpha-secure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Cyber Insurance
- Insurance
- InsurTech
- Endpoint Security
- Managed Detection and Response
- Email Security
- Backup and Recovery
- Risk Management
- Small Business
---
