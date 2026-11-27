---
api_specs:
- filename: multilocale-com-phrases-api-openapi.yml
  format: yaml
  label: MultiLocale Phrases API
  slug: multilocale-com-phrases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multilocale-com/openapi/multilocale-com-phrases-api-openapi.yml
- filename: multilocale-com-projects-api-openapi.yml
  format: yaml
  label: MultiLocale Projects API
  slug: multilocale-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multilocale-com/openapi/multilocale-com-projects-api-openapi.yml
- filename: multilocale-com-sandbox-api-openapi.yml
  format: yaml
  label: MultiLocale Sandbox API
  slug: multilocale-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multilocale-com/openapi/multilocale-com-sandbox-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: multilocale.com
  spf: true
hosts:
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: multilocale.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MultiLocale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MultiLocale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MultiLocale
provider_slug: multilocale-com
slug: multilocale-com-domain-security
source_filename: multilocale-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: multilocale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: multilocale.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/multilocale-com/security/multilocale-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Localization
- Translation
- Developer Tools
- Software-as-a-Service
---
