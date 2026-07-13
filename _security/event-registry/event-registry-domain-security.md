---
api_specs:
- filename: documentation
  format: yaml
  label: Event Registry News API
  slug: news-api
  spec_type: OpenAPI
  url: https://newsapi.ai/documentation
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eventregistry.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: newsapi.ai
  spf: false
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: eventregistry.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: newsapi.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Event Registry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Event Registry, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Event Registry
provider_slug: event-registry
slug: event-registry-domain-security
source_filename: event-registry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eventregistry.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: newsapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eventregistry.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: newsapi.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/event-registry/refs/heads/main/security/event-registry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- News
- Media Monitoring
- News Intelligence
- Event Detection
- Named Entity Recognition
- Sentiment Analysis
- Media Analytics
- News API
---
