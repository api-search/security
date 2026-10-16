---
description: ''
domains:
- caa:
  - 128 iodef "mailto:cert@polisen.se"
  - 128 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: polisen.se
  spf: true
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: polisen.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Polisen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polisen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Polisen
provider_slug: polisen
slug: polisen-domain-security
source_filename: polisen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polisen.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: polisen.se\n  dnssec: true\n  caa:\n  - 128 iodef \"mailto:cert@polisen.se\"\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polisen/refs/heads/main/security/polisen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Government
- Law Enforcement
- Public Safety
- Sweden
---
