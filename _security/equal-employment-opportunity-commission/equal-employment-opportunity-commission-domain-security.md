---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eeoc.gov
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.eeoc.gov
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Equal Employment Opportunity Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Equal Employment Opportunity Commission, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Equal Employment Opportunity Commission
provider_slug: equal-employment-opportunity-commission
slug: equal-employment-opportunity-commission-domain-security
source_filename: equal-employment-opportunity-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eeoc.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eeoc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equal-employment-opportunity-commission/refs/heads/main/security/equal-employment-opportunity-commission-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Labor
- Employment
- Civil Rights
- Open Data
---
