---
api_specs:
- filename: campaignstack-io-openapi-generated.yml
  format: yaml
  label: CampaignStack API
  slug: campaignstack-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/campaignstack-io/openapi/_ae-authored/campaignstack-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: campaignstack.io
  spf: true
hosts:
- cert_expires: Jan  1 18:24:05 2027 GMT
  host: campaignstack.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Campaignstack Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CampaignStack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CampaignStack
provider_slug: campaignstack-io
slug: campaignstack-io-domain-security
source_filename: campaignstack-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: campaignstack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 18:24:05 2027 GMT\n  hsts: false\ndomains:\n- domain: campaignstack.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/campaignstack-io/security/campaignstack-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Outbound outreach
- LinkedIn sourcing
- B2B SaaS
---
