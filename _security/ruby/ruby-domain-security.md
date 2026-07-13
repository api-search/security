---
api_specs:
- filename: rubygems-registry-openapi.yml
  format: yaml
  label: RubyGems.org Registry API v1
  slug: rubygems-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ruby/refs/heads/main/openapi/rubygems-registry-openapi.yml
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
