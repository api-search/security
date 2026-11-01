---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: donorsearch.net
  spf: true
hosts:
- cert_expires: Dec 15 02:33:30 2026 GMT
  host: donorsearch.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Donorsearch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DonorSearch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DonorSearch
provider_slug: donorsearch
slug: donorsearch-domain-security
source_filename: donorsearch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: donorsearch.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 02:33:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: donorsearch.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/donorsearch/security/donorsearch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Nonprofit
- Fundraising
- DonorResearch
- API
---
