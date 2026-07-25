---
api_specs:
- filename: ruby-activity-api-openapi.yml
  format: yaml
  label: Ruby Programming Language and Popular API Gems Activity API
  slug: ruby-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ruby/refs/heads/main/openapi/ruby-activity-api-openapi.yml
- filename: ruby-api-keys-api-openapi.yml
  format: yaml
  label: Ruby Programming Language and Popular API Gems API Keys API
  slug: ruby-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ruby/refs/heads/main/openapi/ruby-api-keys-api-openapi.yml
- filename: ruby-downloads-api-openapi.yml
  format: yaml
  label: Ruby Programming Language and Popular API Gems Downloads API
  slug: ruby-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ruby/refs/heads/main/openapi/ruby-downloads-api-openapi.yml
- filename: ruby-gems-api-openapi.yml
  format: yaml
  label: Ruby Programming Language and Popular API Gems Gems API
  slug: ruby-gems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ruby/refs/heads/main/openapi/ruby-gems-api-openapi.yml
- filename: ruby-oidc-api-openapi.yml
  format: yaml
  label: Ruby Programming Language and Popular API Gems OIDC API
  slug: ruby-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ruby/refs/heads/main/openapi/ruby-oidc-api-openapi.yml
- filename: ruby-owners-api-openapi.yml
  format: yaml
  label: Ruby Programming Language and Popular API Gems Owners API
  slug: ruby-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ruby/refs/heads/main/openapi/ruby-owners-api-openapi.yml
- filename: ruby-profiles-api-openapi.yml
  format: yaml
  label: Ruby Programming Language and Popular API Gems Profiles API
  slug: ruby-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ruby/refs/heads/main/openapi/ruby-profiles-api-openapi.yml
- filename: ruby-versions-api-openapi.yml
  format: yaml
  label: Ruby Programming Language and Popular API Gems Versions API
  slug: ruby-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ruby/refs/heads/main/openapi/ruby-versions-api-openapi.yml
- filename: ruby-webhooks-api-openapi.yml
  format: yaml
  label: Ruby Programming Language and Popular API Gems Webhooks API
  slug: ruby-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ruby/refs/heads/main/openapi/ruby-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ruby-lang.org
  spf: true
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "globalsign.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rubygems.org
  spf: true
hosts:
- cert_expires: Sep 23 11:51:18 2026 GMT
  host: www.ruby-lang.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 00:28:08 2027 GMT
  host: docs.ruby-lang.org
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 17 19:11:19 2026 GMT
  host: guides.rubygems.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ruby Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ruby Programming Language and Popular API Gems, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ruby Programming Language and Popular API Gems
provider_slug: ruby
slug: ruby-domain-security
source_filename: ruby-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ruby-lang.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 11:51:18 2026 GMT\n  hsts: false\n- host: docs.ruby-lang.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 10 00:28:08 2027 GMT\n  hsts: false\n- host: guides.rubygems.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:11:19 2026 GMT\n  hsts: false\ndomains:\n- domain: ruby-lang.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rubygems.org\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ruby/refs/heads/main/security/ruby-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Programming Language
- Ruby
- HTTP
- REST
- API Clients
- Frameworks
- Libraries
- Package Registry
---
