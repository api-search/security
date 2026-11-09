---
api_specs:
- filename: fastsocial-co-profiles-api-openapi.yml
  format: yaml
  label: FastSocial Profiles API
  slug: fastsocial-co-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastsocial-co/openapi/fastsocial-co-profiles-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fastsocial.co
  spf: true
hosts:
- cert_expires: Jan 11 16:46:05 2027 GMT
  host: fastsocial.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fastsocial Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FastSocial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FastSocial
provider_slug: fastsocial-co
slug: fastsocial-co-domain-security
source_filename: fastsocial-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fastsocial.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 16:46:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fastsocial.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fastsocial-co/security/fastsocial-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Media
- Marketing
- API
- Instagram
- FastSocial
---
