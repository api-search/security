---
api_specs:
- filename: bioaegis-therapeutics-blocks-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Blocks API
  slug: bioaegis-therapeutics-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-blocks-api-openapi.yml
- filename: bioaegis-therapeutics-comments-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Comments API
  slug: bioaegis-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-comments-api-openapi.yml
- filename: bioaegis-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Discovery API
  slug: bioaegis-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-discovery-api-openapi.yml
- filename: bioaegis-therapeutics-media-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Media API
  slug: bioaegis-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-media-api-openapi.yml
- filename: bioaegis-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Oembed API
  slug: bioaegis-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-oembed-api-openapi.yml
- filename: bioaegis-therapeutics-pages-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Pages API
  slug: bioaegis-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-pages-api-openapi.yml
- filename: bioaegis-therapeutics-posts-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Posts API
  slug: bioaegis-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-posts-api-openapi.yml
- filename: bioaegis-therapeutics-search-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Search API
  slug: bioaegis-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-search-api-openapi.yml
- filename: bioaegis-therapeutics-seo-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Seo API
  slug: bioaegis-therapeutics-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-seo-api-openapi.yml
- filename: bioaegis-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: BioAegis Therapeutics Taxonomy API
  slug: bioaegis-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/openapi/bioaegis-therapeutics-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bioaegistherapeutics.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  - 0 iodef "mailto:caa@wordpress.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Sep 29 08:17:12 2026 GMT
  host: www.bioaegistherapeutics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 19:43:55 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bioaegis Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BioAegis Therapeutics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BioAegis Therapeutics
provider_slug: bioaegis-therapeutics
slug: bioaegis-therapeutics-domain-security
source_filename: bioaegis-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bioaegistherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 08:17:12 2026 GMT\n  hsts: false\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: bioaegistherapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/security/bioaegis-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- biopharmaceuticals
- biotechnology
- clinical-trials
- immunology
- inflammation
- innate-immunity
- gelsolin
- protein-therapeutics
- ards
- critical-care
- rare-disease
- drug-development
- life-sciences
- content-api
---
