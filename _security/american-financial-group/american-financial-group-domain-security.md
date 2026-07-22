---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: afginc.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: greatamericaninsurancegroup.com
  spf: true
hosts:
- cert_expires: Aug 18 02:28:54 2026 GMT
  host: www.afginc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:44:41 2026 GMT
  host: www.greatamericaninsurancegroup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: American Financial Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for American Financial Group, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: American Financial Group
provider_slug: american-financial-group
slug: american-financial-group-domain-security
source_filename: american-financial-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.afginc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 02:28:54 2026 GMT\n  hsts: null\n- host: www.greatamericaninsurancegroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:44:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: afginc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: greatamericaninsurancegroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-financial-group/refs/heads/main/security/american-financial-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Property Casualty
- Specialty Insurance
- Annuities
- Financial Services
- Commercial Insurance
- Fortune 500
---
