---
api_specs:
- filename: amazon-relay-openapi-generated.yml
  format: yaml
  label: Amazon Relay API
  slug: amazon-relay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-relay/openapi/_ae-authored/amazon-relay-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: relay.amazon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amazon Relay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Relay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Relay
provider_slug: amazon-relay
slug: amazon-relay-domain-security
source_filename: amazon-relay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: relay.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-relay/security/amazon-relay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Logistics
- Freight
- Transportation
- Carrier
---
