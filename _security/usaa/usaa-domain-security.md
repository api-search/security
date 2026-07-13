---
description: ''
domains:
- caa:
  - 0 iodef "mailto:usaadomains@usaa.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usaa.com
  spf: true
hosts:
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: www.usaa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Usaa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for USAA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: USAA
provider_slug: usaa
slug: usaa-domain-security
source_filename: usaa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usaa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usaa.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:usaadomains@usaa.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usaa/refs/heads/main/security/usaa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- Insurance
- Military Finance
- Open Banking
- Fortune 100
---
