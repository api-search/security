---
api_specs:
- filename: clojars-artifacts-api-openapi.yml
  format: yaml
  label: Clojars Artifacts API
  slug: clojars-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clojars/refs/heads/main/openapi/clojars-artifacts-api-openapi.yml
- filename: clojars-feeds-api-openapi.yml
  format: yaml
  label: Clojars Feeds API
  slug: clojars-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clojars/refs/heads/main/openapi/clojars-feeds-api-openapi.yml
- filename: clojars-groups-api-openapi.yml
  format: yaml
  label: Clojars Groups API
  slug: clojars-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clojars/refs/heads/main/openapi/clojars-groups-api-openapi.yml
- filename: clojars-search-api-openapi.yml
  format: yaml
  label: Clojars Search API
  slug: clojars-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clojars/refs/heads/main/openapi/clojars-search-api-openapi.yml
- filename: clojars-users-api-openapi.yml
  format: yaml
  label: Clojars Users API
  slug: clojars-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clojars/refs/heads/main/openapi/clojars-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clojars.org
  spf: true
hosts:
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: clojars.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clojars Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clojars, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clojars
provider_slug: clojars
slug: clojars-domain-security
source_filename: clojars-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clojars.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clojars.org\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clojars/refs/heads/main/security/clojars-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Clojure
- Package Registry
- Artifact Repository
- Open-Source
---
