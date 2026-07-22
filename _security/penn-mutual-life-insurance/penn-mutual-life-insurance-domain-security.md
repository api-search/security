---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pennmutual.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: www.pennmutual.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Penn Mutual Life Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Penn Mutual Life Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Penn Mutual Life Insurance
provider_slug: penn-mutual-life-insurance
slug: penn-mutual-life-insurance-domain-security
source_filename: penn-mutual-life-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pennmutual.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: pennmutual.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/penn-mutual-life-insurance/refs/heads/main/security/penn-mutual-life-insurance-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- Life Insurance
- Annuities
- Financial Services
---
