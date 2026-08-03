---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: thoughtmachine.net
  spf: true
hosts:
- cert_expires: Oct 21 04:13:43 2026 GMT
  host: www.thoughtmachine.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 00:13:13 2026 GMT
  host: docs.thoughtmachine.net
  hsts: false
  https: true
  note: 302 redirect to auth.thoughtmachine.net SSO (partner login required)
  tls_version: TLSv1.3
- cert_expires: Sep 30 16:29:03 2026 GMT
  host: portal.thoughtmachine.net
  hsts: false
  https: true
  note: 302 redirect to auth.thoughtmachine.net SSO (enablement portal)
  tls_version: TLSv1.3
- cert_expires: Oct  4 03:57:33 2026 GMT
  host: auth.thoughtmachine.net
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thought Machine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thought Machine, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Thought Machine
provider_slug: thought-machine
slug: thought-machine-domain-security
source_filename: thought-machine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thoughtmachine.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 04:13:43 2026 GMT\n  hsts: false\n- host: docs.thoughtmachine.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 00:13:13 2026 GMT\n  hsts: false\n  note: 302 redirect to auth.thoughtmachine.net SSO (partner login required)\n- host: portal.thoughtmachine.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:29:03 2026 GMT\n  hsts: false\n  note: 302 redirect to auth.thoughtmachine.net SSO (enablement portal)\n- host: auth.thoughtmachine.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 03:57:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\ndomains:\n- domain: thoughtmachine.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thought-machine/refs/heads/main/security/thought-machine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Banking
- Core Banking
- Financial Services
- Payments
- Cloud Native
- Smart Contracts
- ISO 20022
- Ledger
- Fintech
- United Kingdom
---
