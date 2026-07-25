---
api_specs:
- filename: r-badges-api-openapi.yml
  format: yaml
  label: R Badges API
  slug: r-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/r/refs/heads/main/openapi/r-badges-api-openapi.yml
- filename: r-downloads-api-openapi.yml
  format: yaml
  label: R Downloads API
  slug: r-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/r/refs/heads/main/openapi/r-downloads-api-openapi.yml
- filename: r-packages-api-openapi.yml
  format: yaml
  label: R Packages API
  slug: r-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/r/refs/heads/main/openapi/r-packages-api-openapi.yml
- filename: r-top-packages-api-openapi.yml
  format: yaml
  label: R Top Packages API
  slug: r-top-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/r/refs/heads/main/openapi/r-top-packages-api-openapi.yml
- filename: r-versions-api-openapi.yml
  format: yaml
  label: R Versions API
  slug: r-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/r/refs/heads/main/openapi/r-versions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: r-project.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: r-pkg.org
  spf: true
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: www.r-project.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 11:58:52 2026 GMT
  host: crandb.r-pkg.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 11:58:52 2026 GMT
  host: cranlogs.r-pkg.org
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: R Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for R, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: R
provider_slug: r
slug: r-domain-security
source_filename: r-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.r-project.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: false\n- host: crandb.r-pkg.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 11:58:52 2026 GMT\n  hsts: false\n- host: cranlogs.r-pkg.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 11:58:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: r-project.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: r-pkg.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/r/refs/heads/main/security/r-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- R
- Statistics
- Data Science
- Open Source
- Programming Language
---
