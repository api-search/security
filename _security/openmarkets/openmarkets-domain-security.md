---
api_specs:
- filename: openmarkets-openapi-generated.yml
  format: yaml
  label: OpenMarkets Group API
  slug: openmarkets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmarkets/openapi/_ae-authored/openmarkets-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: openmarkets.com.au
  spf: true
hosts:
- cert_expires: Jan 16 01:03:39 2027 GMT
  host: openmarkets.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Openmarkets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenMarkets Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: OpenMarkets Group
provider_slug: openmarkets
slug: openmarkets-domain-security
source_filename: openmarkets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openmarkets.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 01:03:39 2027 GMT\n  hsts: false\ndomains:\n- domain: openmarkets.com.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/openmarkets/security/openmarkets-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
