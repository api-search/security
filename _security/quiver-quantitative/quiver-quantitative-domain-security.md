---
api_specs:
- filename: quiver-quantitative-beta-api-openapi.yml
  format: yaml
  label: Quiver Quantitative Beta API
  slug: quiver-quantitative-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiver-quantitative/refs/heads/main/openapi/quiver-quantitative-beta-api-openapi.yml
- filename: quiver-quantitative-tier-1-api-openapi.yml
  format: yaml
  label: Quiver Quantitative Tier 1 API
  slug: quiver-quantitative-tier-1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiver-quantitative/refs/heads/main/openapi/quiver-quantitative-tier-1-api-openapi.yml
- filename: quiver-quantitative-tier-2-api-openapi.yml
  format: yaml
  label: Quiver Quantitative Tier 2 API
  slug: quiver-quantitative-tier-2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiver-quantitative/refs/heads/main/openapi/quiver-quantitative-tier-2-api-openapi.yml
- filename: quiver-quantitative-tier-new-constructs-ratings-api-openapi.yml
  format: yaml
  label: Quiver Quantitative Tier New Constructs Ratings API
  slug: quiver-quantitative-tier-new-constructs-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiver-quantitative/refs/heads/main/openapi/quiver-quantitative-tier-new-constructs-ratings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quiverquant.com
  spf: true
hosts:
- cert_expires: Dec  4 05:46:06 2026 GMT
  host: www.quiverquant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Quiver Quantitative Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quiver Quantitative, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Quiver Quantitative
provider_slug: quiver-quantitative
slug: quiver-quantitative-domain-security
source_filename: quiver-quantitative-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quiverquant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 05:46:06 2026 GMT\n  hsts: false\ndomains:\n- domain: quiverquant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quiver-quantitative/refs/heads/main/security/quiver-quantitative-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data
- Finance
- Politics
---
