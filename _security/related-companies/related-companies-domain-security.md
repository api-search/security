---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: related.com
  spf: true
hosts:
- cert_expires: Aug 24 15:16:03 2026 GMT
  host: www.related.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Related Companies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Related Companies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Related Companies
provider_slug: related-companies
slug: related-companies-domain-security
source_filename: related-companies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.related.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 15:16:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: related.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/related-companies/refs/heads/main/security/related-companies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Real Estate Development
- Residential
- Affordable Housing
- Mixed Use Development
- Commercial Real Estate
- Retail
- Hospitality
- Data Centers
---
