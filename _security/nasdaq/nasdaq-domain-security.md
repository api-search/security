---
api_specs:
- filename: nasdaq-asyncapi.yml
  format: yaml
  label: Nasdaq Cloud Data Service (NCDS) — Kafka Streams
  slug: nasdaq-cloud-data-service-ncds-kafka-streams
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasdaq/refs/heads/main/asyncapi/nasdaq-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nasdaq.com
  spf: true
hosts:
- host: streams.ncds.nasdaq.com
  https: false
kind: domain-security
layout: security
method: probed
name: Nasdaq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nasdaq, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nasdaq
provider_slug: nasdaq
slug: nasdaq-domain-security
source_filename: nasdaq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: streams.ncds.nasdaq.com\n  https: false\ndomains:\n- domain: nasdaq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasdaq/refs/heads/main/security/nasdaq-domain-security.yml
summary_line: DMARC
tags:
- Fortune 1000
---
