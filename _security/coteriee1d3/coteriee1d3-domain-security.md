---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coterieinsurance.com
  spf: true
hosts:
- cert_expires: Nov 19 17:28:42 2026 GMT
  host: coterieinsurance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coteriee1D3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coteriee1d3, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coteriee1d3
provider_slug: coteriee1d3
slug: coteriee1d3-domain-security
source_filename: coteriee1d3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coterieinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 17:28:42 2026 GMT\n  hsts: false\ndomains:\n- domain: coterieinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coteriee1d3/refs/heads/main/security/coteriee1d3-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- Small Business
- Fintech
- Software-as-a-Service
- Company
---
