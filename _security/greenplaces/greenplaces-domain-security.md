---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: greenplaces.com
  spf: true
hosts:
- cert_expires: Sep 13 18:43:08 2026 GMT
  host: greenplaces.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Greenplaces Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greenplaces, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Greenplaces
provider_slug: greenplaces
slug: greenplaces-domain-security
source_filename: greenplaces-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: greenplaces.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:43:08 2026 GMT\n  hsts: false\ndomains:\n- domain: greenplaces.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenplaces/refs/heads/main/security/greenplaces-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sustainability
- ESG
- Carbon Accounting
- Carbon Footprint
- GHG Protocol
- Compliance
- Reporting
- Regulatory
---
