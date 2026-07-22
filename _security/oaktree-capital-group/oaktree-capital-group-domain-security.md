---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oaktreecapital.com
  spf: true
hosts:
- cert_expires: Sep 15 07:06:01 2026 GMT
  host: www.oaktreecapital.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oaktree Capital Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oaktree Capital Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oaktree Capital Group
provider_slug: oaktree-capital-group
slug: oaktree-capital-group-domain-security
source_filename: oaktree-capital-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oaktreecapital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:06:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oaktreecapital.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oaktree-capital-group/refs/heads/main/security/oaktree-capital-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Asset Management
- Capital
- Credit
- Finance
- Investment
- Private Equity
- Fortune 1000
---
