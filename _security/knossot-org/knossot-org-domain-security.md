---
api_specs:
- filename: knossot-org-credits-api-openapi.yml
  format: yaml
  label: Knossot Credits API
  slug: knossot-org-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knossot-org/openapi/knossot-org-credits-api-openapi.yml
- filename: knossot-org-keys-api-openapi.yml
  format: yaml
  label: Knossot Keys API
  slug: knossot-org-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knossot-org/openapi/knossot-org-keys-api-openapi.yml
- filename: knossot-org-knossot-agent-api-api-openapi.yml
  format: yaml
  label: Knossot Knossot Agent API
  slug: knossot-org-knossot-agent-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knossot-org/openapi/knossot-org-knossot-agent-api-api-openapi.yml
- filename: knossot-org-recommendations-api-openapi.yml
  format: yaml
  label: Knossot Recommendations API
  slug: knossot-org-recommendations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knossot-org/openapi/knossot-org-recommendations-api-openapi.yml
- filename: knossot-org-regions-api-openapi.yml
  format: yaml
  label: Knossot Regions API
  slug: knossot-org-regions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knossot-org/openapi/knossot-org-regions-api-openapi.yml
- filename: knossot-org-usage-api-openapi.yml
  format: yaml
  label: Knossot Usage API
  slug: knossot-org-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knossot-org/openapi/knossot-org-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: knossot.org
  spf: true
hosts:
- cert_expires: Jan 22 23:22:36 2027 GMT
  host: knossot.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Knossot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knossot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Knossot
provider_slug: knossot-org
slug: knossot-org-domain-security
source_filename: knossot-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knossot.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:22:36 2027 GMT\n  hsts: false\ndomains:\n- domain: knossot.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/knossot-org/security/knossot-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Community
- Event
- Calendar
- Hudson Valley
- Non-commercial
---
