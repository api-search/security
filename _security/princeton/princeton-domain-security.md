---
api_specs:
- filename: princeton-art-museum-api-openapi.yml
  format: yaml
  label: Princeton University Art Museum API
  slug: art-museum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-art-museum-api-openapi.yml
- filename: princeton-article-api-openapi.yml
  format: yaml
  label: Princeton University Article API
  slug: princeton-article-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-article-api-openapi.yml
- filename: princeton-banner-api-openapi.yml
  format: yaml
  label: Princeton University Banner API
  slug: princeton-banner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-banner-api-openapi.yml
- filename: princeton-best-bets-api-openapi.yml
  format: yaml
  label: Princeton University Best Bets API
  slug: princeton-best-bets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-best-bets-api-openapi.yml
- filename: princeton-catalog-api-openapi.yml
  format: yaml
  label: Princeton University Catalog API
  slug: princeton-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-catalog-api-openapi.yml
- filename: princeton-dpul-api-openapi.yml
  format: yaml
  label: Princeton University Dpul API
  slug: princeton-dpul-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-dpul-api-openapi.yml
- filename: princeton-findingaids-api-openapi.yml
  format: yaml
  label: Princeton University Findingaids API
  slug: princeton-findingaids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-findingaids-api-openapi.yml
- filename: princeton-journals-api-openapi.yml
  format: yaml
  label: Princeton University Journals API
  slug: princeton-journals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-journals-api-openapi.yml
- filename: princeton-libanswers-api-openapi.yml
  format: yaml
  label: Princeton University Libanswers API
  slug: princeton-libanswers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-libanswers-api-openapi.yml
- filename: princeton-libguides-api-openapi.yml
  format: yaml
  label: Princeton University Libguides API
  slug: princeton-libguides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-libguides-api-openapi.yml
- filename: princeton-library-databases-api-openapi.yml
  format: yaml
  label: Princeton University Library Databases API
  slug: princeton-library-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-library-databases-api-openapi.yml
- filename: princeton-library-staff-api-openapi.yml
  format: yaml
  label: Princeton University Library Staff API
  slug: princeton-library-staff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-library-staff-api-openapi.yml
- filename: princeton-library-website-api-openapi.yml
  format: yaml
  label: Princeton University Library Website API
  slug: princeton-library-website-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-library-website-api-openapi.yml
- filename: princeton-makers-api-openapi.yml
  format: yaml
  label: Princeton University Makers API
  slug: princeton-makers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-makers-api-openapi.yml
- filename: princeton-objects-api-openapi.yml
  format: yaml
  label: Princeton University Objects API
  slug: princeton-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-objects-api-openapi.yml
- filename: princeton-packages-api-openapi.yml
  format: yaml
  label: Princeton University Packages API
  slug: princeton-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-packages-api-openapi.yml
- filename: princeton-pulmap-api-openapi.yml
  format: yaml
  label: Princeton University Pulmap API
  slug: princeton-pulmap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-pulmap-api-openapi.yml
- filename: princeton-search-api-openapi.yml
  format: yaml
  label: Princeton University Search API
  slug: princeton-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: princeton.edu
  spf: true
hosts:
- cert_expires: Aug 30 00:57:27 2026 GMT
  host: www.princeton.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 23:59:59 2026 GMT
  host: data.artmuseum.princeton.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api-store.princeton.edu
  https: false
kind: domain-security
layout: security
method: probed
name: Princeton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Princeton University, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Princeton University
provider_slug: princeton
slug: princeton-domain-security
source_filename: princeton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.princeton.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 00:57:27 2026 GMT\n  hsts: false\n- host: data.artmuseum.princeton.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:59:59 2026 GMT\n  hsts: null\n- host: api-store.princeton.edu\n  https: false\ndomains:\n- domain: princeton.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/security/princeton-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- University
- Higher Education
- Education
- Ivy League
- United States
- New Jersey
- Research Library
- Research Data
- Open Data
- Digital Collections
- Identity Federation
- Museum
---
