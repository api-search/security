---
api_specs:
- filename: heymarvin-openapi-generated.yml
  format: yaml
  label: HeyMarvin API
  slug: heymarvin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heymarvin/openapi/_ae-authored/heymarvin-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com "
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: heymarvin.com
  spf: true
hosts:
- cert_expires: Dec 17 09:32:30 2026 GMT
  host: heymarvin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Heymarvin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HeyMarvin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HeyMarvin
provider_slug: heymarvin
slug: heymarvin-domain-security
source_filename: heymarvin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heymarvin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 09:32:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heymarvin.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com \"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/heymarvin/security/heymarvin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- CustomerInsights
- Analytics
- SaaS
- Platform
---
