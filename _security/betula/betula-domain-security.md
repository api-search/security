---
api_specs:
- filename: betula-betula-api-api-openapi.yml
  format: yaml
  label: Betula API
  slug: betula-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/betula/openapi/betula-betula-api-api-openapi.yml
- filename: betula-openapi-generated.yml
  format: yaml
  label: Betula API
  slug: betula-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/betula/openapi/_ae-authored/betula-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: joinbetula.org
  spf: false
hosts:
- cert_expires: Jan  8 15:51:28 2027 GMT
  host: joinbetula.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Betula Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Betula, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Betula
provider_slug: betula
slug: betula-domain-security
source_filename: betula-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joinbetula.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 15:51:28 2027 GMT\n  hsts: false\ndomains:\n- domain: joinbetula.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/betula/security/betula-domain-security.yml
summary_line: TLSv1.3
tags:
- Bookmark Manager
- Federated
- Open Source
- Self-hosted
- Independent Web
- Company
---
