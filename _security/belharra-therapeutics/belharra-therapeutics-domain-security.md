---
api_specs:
- filename: belharra-therapeutics-custom-types-api-openapi.yml
  format: yaml
  label: Belharra Therapeutics Custom Types API
  slug: belharra-therapeutics-custom-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/openapi/belharra-therapeutics-custom-types-api-openapi.yml
- filename: belharra-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Belharra Therapeutics Discovery API
  slug: belharra-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/openapi/belharra-therapeutics-discovery-api-openapi.yml
- filename: belharra-therapeutics-media-api-openapi.yml
  format: yaml
  label: Belharra Therapeutics Media API
  slug: belharra-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/openapi/belharra-therapeutics-media-api-openapi.yml
- filename: belharra-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Belharra Therapeutics Oembed API
  slug: belharra-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/openapi/belharra-therapeutics-oembed-api-openapi.yml
- filename: belharra-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Belharra Therapeutics Pages API
  slug: belharra-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/openapi/belharra-therapeutics-pages-api-openapi.yml
- filename: belharra-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Belharra Therapeutics Posts API
  slug: belharra-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/openapi/belharra-therapeutics-posts-api-openapi.yml
- filename: belharra-therapeutics-search-api-openapi.yml
  format: yaml
  label: Belharra Therapeutics Search API
  slug: belharra-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/openapi/belharra-therapeutics-search-api-openapi.yml
- filename: belharra-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Belharra Therapeutics Taxonomy API
  slug: belharra-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/openapi/belharra-therapeutics-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: belharratx.com
  spf: true
- caa:
  - 0 iodef "mailto:caa@wordpress.org"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Sep 30 20:02:48 2026 GMT
  host: belharratx.com
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
name: Belharra Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Belharra Therapeutics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Belharra Therapeutics
provider_slug: belharra-therapeutics
slug: belharra-therapeutics-domain-security
source_filename: belharra-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: belharratx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 20:02:48 2026 GMT\n  hsts: false\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: belharratx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/belharra-therapeutics/refs/heads/main/security/belharra-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Chemoproteomics
- Drug Discovery
- Small Molecule Therapeutics
- Proteomics
- Life Sciences
- Oncology
- Immunology
- content-api
---
