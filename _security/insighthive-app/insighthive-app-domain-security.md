---
api_specs:
- filename: insighthive-app-api-openapi.yml
  format: yaml
  label: Insight Hive Watchlist API API
  slug: insight-hive-watchlist-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insighthive-app/openapi/_original/insighthive-app-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: insighthive.app
  spf: true
hosts:
- cert_expires: Jan 26 04:32:02 2027 GMT
  host: insighthive.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Insight Hive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insight Hive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Insight Hive
provider_slug: insighthive-app
slug: insighthive-app-domain-security
source_filename: insighthive-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insighthive.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 04:32:02 2027 GMT\n  hsts: false\ndomains:\n- domain: insighthive.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/insighthive-app/security/insighthive-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Social Media
- Scheduling
- Competitor Analysis
- Software-as-a-Service
---
