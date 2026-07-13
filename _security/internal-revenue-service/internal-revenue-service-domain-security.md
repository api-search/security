---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: irs.gov
  spf: true
hosts:
- cert_expires: Aug 24 05:55:53 2026 GMT
  host: www.irs.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Internal Revenue Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Internal Revenue Service, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Internal Revenue Service
provider_slug: internal-revenue-service
slug: internal-revenue-service-domain-security
source_filename: internal-revenue-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.irs.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 05:55:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: irs.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/internal-revenue-service/refs/heads/main/security/internal-revenue-service-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Finance
- IRS
- Tax
- Tax Filing
---
