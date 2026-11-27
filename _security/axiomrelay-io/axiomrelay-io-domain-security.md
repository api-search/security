---
api_specs:
- filename: axiomrelay-io-agents-api-openapi.yml
  format: yaml
  label: Axiom Relay Agents API
  slug: axiomrelay-io-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-agents-api-openapi.yml
- filename: axiomrelay-io-capabilities-api-openapi.yml
  format: yaml
  label: Axiom Relay Capabilities API
  slug: axiomrelay-io-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-capabilities-api-openapi.yml
- filename: axiomrelay-io-commerce-api-openapi.yml
  format: yaml
  label: Axiom Relay Commerce API
  slug: axiomrelay-io-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-commerce-api-openapi.yml
- filename: axiomrelay-io-commons-api-openapi.yml
  format: yaml
  label: Axiom Relay Commons API
  slug: axiomrelay-io-commons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-commons-api-openapi.yml
- filename: axiomrelay-io-communications-api-openapi.yml
  format: yaml
  label: Axiom Relay Communications API
  slug: axiomrelay-io-communications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-communications-api-openapi.yml
- filename: axiomrelay-io-directory-api-openapi.yml
  format: yaml
  label: Axiom Relay Directory API
  slug: axiomrelay-io-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-directory-api-openapi.yml
- filename: axiomrelay-io-evidence-api-openapi.yml
  format: yaml
  label: Axiom Relay Evidence API
  slug: axiomrelay-io-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-evidence-api-openapi.yml
- filename: axiomrelay-io-health-api-openapi.yml
  format: yaml
  label: Axiom Relay Health API
  slug: axiomrelay-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-health-api-openapi.yml
- filename: axiomrelay-io-payments-api-openapi.yml
  format: yaml
  label: Axiom Relay Payments API
  slug: axiomrelay-io-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-payments-api-openapi.yml
- filename: axiomrelay-io-platform-api-openapi.yml
  format: yaml
  label: Axiom Relay Platform API
  slug: axiomrelay-io-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-platform-api-openapi.yml
- filename: axiomrelay-io-treasury-api-openapi.yml
  format: yaml
  label: Axiom Relay Treasury API
  slug: axiomrelay-io-treasury-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomrelay-io/openapi/axiomrelay-io-treasury-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: axiomrelay.io
  spf: false
hosts:
- cert_expires: Jan 24 01:09:49 2027 GMT
  host: axiomrelay.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Axiom Relay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axiom Relay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Axiom Relay
provider_slug: axiomrelay-io
slug: axiomrelay-io-domain-security
source_filename: axiomrelay-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axiomrelay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 01:09:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: axiomrelay.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/axiomrelay-io/security/axiomrelay-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- Commerce
- Marketplace
- Infrastructure
---
