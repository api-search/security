---
api_specs:
- filename: rubygems-gems-api-openapi.yml
  format: yaml
  label: RubyGems Gems API
  slug: gems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-gems-api-openapi.yml
- filename: rubygems-api-v2-openapi.yml
  format: yaml
  label: RubyGems API V2
  slug: api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-api-v2-openapi.yml
- filename: rubygems-downloads-api-openapi.yml
  format: yaml
  label: RubyGems Downloads API
  slug: downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-downloads-api-openapi.yml
- filename: rubygems-search-api-openapi.yml
  format: yaml
  label: RubyGems Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-search-api-openapi.yml
- filename: rubygems-activity-api-openapi.yml
  format: yaml
  label: RubyGems Activity API
  slug: activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-activity-api-openapi.yml
- filename: rubygems-webhooks-api-openapi.yml
  format: yaml
  label: RubyGems Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/openapi/rubygems-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "globalsign.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rubygems.org
  spf: true
hosts:
- cert_expires: Mar  9 18:00:25 2027 GMT
  host: rubygems.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 19:11:19 2026 GMT
  host: guides.rubygems.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rubygems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RubyGems, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RubyGems
provider_slug: rubygems
slug: rubygems-domain-security
source_filename: rubygems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rubygems.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 18:00:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: guides.rubygems.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:11:19 2026 GMT\n  hsts: false\ndomains:\n- domain: rubygems.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/security/rubygems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ruby
- Package Manager
- Open Source
- Developer Tools
---
