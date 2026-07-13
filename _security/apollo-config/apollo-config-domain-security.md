---
api_specs:
- filename: apollo-open-api.yml
  format: yaml
  label: Apollo Config
  slug: apollo-config
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-config/refs/heads/main/openapi/apollo-open-api.yml
description: ''
domains:
- caa:
  - apolloconfig.github.io.
  - 0 issuewild "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  dmarc: false
  dnssec: true
  domain: apolloconfig.com
  spf: false
hosts:
- cert_expires: Sep 27 16:36:56 2026 GMT
  host: www.apolloconfig.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apollo Config Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apollo Config, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Apollo Config
provider_slug: apollo-config
slug: apollo-config-domain-security
source_filename: apollo-config-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apolloconfig.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:36:56 2026 GMT\n  hsts: false\ndomains:\n- domain: apolloconfig.com\n  dnssec: true\n  caa:\n  - apolloconfig.github.io.\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-config/refs/heads/main/security/apollo-config-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Apache 2.0
- Configuration Management
- Ctrip
- Distributed Systems
- Java
- Microservices
- Open Source
- Real-Time Configuration
---
