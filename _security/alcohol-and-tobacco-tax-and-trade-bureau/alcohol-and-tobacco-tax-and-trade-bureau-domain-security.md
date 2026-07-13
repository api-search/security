---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ttb.gov
  spf: true
hosts:
- cert_expires: Jul 29 14:50:02 2026 GMT
  host: www.ttb.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alcohol And Tobacco Tax And Trade Bureau Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alcohol and Tobacco Tax and Trade Bureau, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Alcohol and Tobacco Tax and Trade Bureau
provider_slug: alcohol-and-tobacco-tax-and-trade-bureau
slug: alcohol-and-tobacco-tax-and-trade-bureau-domain-security
source_filename: alcohol-and-tobacco-tax-and-trade-bureau-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ttb.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 14:50:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ttb.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alcohol-and-tobacco-tax-and-trade-bureau/refs/heads/main/security/alcohol-and-tobacco-tax-and-trade-bureau-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Alcohol
- Tobacco
- Federal Government
- Excise Tax
- Regulation
- Treasury
---
