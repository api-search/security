---
api_specs:
- filename: crimsoncrawler-com-openapi-generated.yml
  format: yaml
  label: crimsoncrawler-com API
  slug: crimsoncrawler-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crimsoncrawler-com/openapi/_ae-authored/crimsoncrawler-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crimsoncrawler.com
  spf: true
hosts:
- cert_expires: Jan 16 08:20:19 2027 GMT
  host: crimsoncrawler.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crimsoncrawler Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for crimsoncrawler-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: crimsoncrawler-com
provider_slug: crimsoncrawler-com
slug: crimsoncrawler-com-domain-security
source_filename: crimsoncrawler-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crimsoncrawler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 08:20:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crimsoncrawler.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/crimsoncrawler-com/security/crimsoncrawler-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API
- CVE
- Threat-Intelligence
- Security
- Data-API
---
