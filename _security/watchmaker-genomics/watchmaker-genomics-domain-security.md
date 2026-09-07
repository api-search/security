---
api_specs:
- filename: watchmaker-genomics-commerce-rest-swagger.json
  format: json
  label: Watchmaker Genomics Storefront REST API
  slug: watchmaker-genomics-storefront-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchmaker-genomics/refs/heads/main/openapi/watchmaker-genomics-commerce-rest-swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: watchmakergenomics.com
  spf: true
hosts:
- cert_expires: Nov  4 03:02:18 2026 GMT
  host: www.watchmakergenomics.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Watchmaker Genomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Watchmaker Genomics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Watchmaker Genomics
provider_slug: watchmaker-genomics
slug: watchmaker-genomics-domain-security
source_filename: watchmaker-genomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.watchmakergenomics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 03:02:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: watchmakergenomics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/watchmaker-genomics/refs/heads/main/security/watchmaker-genomics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Genomics
- Life Sciences
- Next-Generation Sequencing
- Molecular Diagnostics
- Biotechnology
- Reagents
- Bioinformatics
- E-Commerce
- GraphQL
- Adobe Commerce
---
