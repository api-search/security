---
description: ''
domains:
- caa:
  - 128 issue "sectigo.com"
  - '128 iodef "mailto: iso_support@fanniemae.com"'
  - 128 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fanniemae.com
  spf: true
hosts:
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: www.fanniemae.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fannie Mae Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fannie Mae, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fannie Mae
provider_slug: fannie-mae
slug: fannie-mae-domain-security
source_filename: fannie-mae-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fanniemae.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: fanniemae.com\n  dnssec: false\n  caa:\n  - 128 issue \"sectigo.com\"\n  - '128 iodef \"mailto: iso_support@fanniemae.com\"'\n  - 128 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fannie-mae/refs/heads/main/security/fannie-mae-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Federal Government
- Housing
- Mortgages
- Finance
- GSE
- Fortune 100
---
