---
api_specs:
- filename: idex-onsite-full-feed-api-openapi.yml
  format: yaml
  label: IDEX Onsite Full Feed API
  slug: idex-onsite-full-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diamond-search/refs/heads/main/openapi/idex-onsite-full-feed-api-openapi.yml
- filename: idex-lab-grown-file-api-openapi.yml
  format: yaml
  label: IDEX Lab Grown File API
  slug: idex-lab-grown-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diamond-search/refs/heads/main/openapi/idex-lab-grown-file-api-openapi.yml
- filename: idex-data-report-api-openapi.yml
  format: yaml
  label: IDEX Data Report API
  slug: idex-data-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diamond-search/refs/heads/main/openapi/idex-data-report-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: idexonline.com
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.idexonline.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Diamond Search Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diamond Search, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Diamond Search
provider_slug: diamond-search
slug: diamond-search-domain-security
source_filename: diamond-search-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.idexonline.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: idexonline.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diamond-search/refs/heads/main/security/diamond-search-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Diamonds
- Lab Grown
- Pricing
- Trading
---
