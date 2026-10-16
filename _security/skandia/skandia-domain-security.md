---
description: ''
domains:
- caa:
  - 0 issuevmc "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:administrator@skandia.se"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: skandia.se
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: skandia.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Skandia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skandia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Skandia
provider_slug: skandia
slug: skandia-domain-security
source_filename: skandia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skandia.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: skandia.se\n  dnssec: true\n  caa:\n  - 0 issuevmc \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:administrator@skandia.se\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skandia/refs/heads/main/security/skandia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Pensions
- Insurance
- Banking
---
