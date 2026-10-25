---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "amazontrust.com"
  - 0 issue "amazontrust.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aware.com.au
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: aware.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aware Super Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aware Super, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aware Super
provider_slug: aware-super
slug: aware-super-domain-security
source_filename: aware-super-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aware.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aware.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aware-super/refs/heads/main/security/aware-super-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Superannuation
- Retirement
- Financial Services
- Investments
- Australia
---
