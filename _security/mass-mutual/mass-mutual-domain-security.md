---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: massmutual.com
  spf: true
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: www.massmutual.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mass Mutual Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MassMutual, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MassMutual
provider_slug: mass-mutual
slug: mass-mutual-domain-security
source_filename: mass-mutual-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.massmutual.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: massmutual.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mass-mutual/refs/heads/main/security/mass-mutual-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Annuities
- Financial Services
- Fortune 500
- Insurance
- Investment Management
- Life Insurance
- Retirement
---
