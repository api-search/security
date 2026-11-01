---
api_specs:
- filename: wholechain-connect-api-openapi.yml
  format: yaml
  label: Wholechain Connect API
  slug: wholechain-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-connect-api-openapi.yml
- filename: wholechain-edi-api-openapi.yml
  format: yaml
  label: Wholechain Edi API
  slug: wholechain-edi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-edi-api-openapi.yml
- filename: wholechain-epcis-interface-api-openapi.yml
  format: yaml
  label: Wholechain EPCIS Interface API
  slug: wholechain-epcis-interface-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-epcis-interface-api-openapi.yml
- filename: wholechain-epcis-legacy-interface-api-openapi.yml
  format: yaml
  label: Wholechain EPCIS Legacy Interface API
  slug: wholechain-epcis-legacy-interface-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-epcis-legacy-interface-api-openapi.yml
- filename: wholechain-events-api-openapi.yml
  format: yaml
  label: Wholechain Events API
  slug: wholechain-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-events-api-openapi.yml
- filename: wholechain-externaloauth-api-openapi.yml
  format: yaml
  label: Wholechain External O Auth API
  slug: wholechain-externaloauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-externaloauth-api-openapi.yml
- filename: wholechain-health-api-openapi.yml
  format: yaml
  label: Wholechain Health API
  slug: wholechain-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-health-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wholechain.com
  spf: true
hosts:
- cert_expires: Dec 27 04:51:01 2026 GMT
  host: wholechain.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wholechain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wholechain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wholechain
provider_slug: wholechain
slug: wholechain-domain-security
source_filename: wholechain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wholechain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 04:51:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wholechain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/wholechain/security/wholechain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Supply Chain
- Traceability
- Blockchain
- Food Safety
- Compliance
- GS1
- Logistics
---
