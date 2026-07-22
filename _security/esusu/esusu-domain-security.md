---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: esusurent.com
  spf: true
hosts:
- cert_expires: Aug 19 08:48:09 2026 GMT
  host: www.esusurent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Esusu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Esusu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Esusu
provider_slug: esusu
slug: esusu-domain-security
source_filename: esusu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.esusurent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 08:48:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: esusurent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esusu/refs/heads/main/security/esusu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Fintech
- Financial Services
- Credit
- Credit Building
- Rent Reporting
- Real Estate
- Identity Verification
- Income Verification
---
