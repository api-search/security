---
api_specs:
- filename: dnsdoctor-dev-domains-api-openapi.yml
  format: yaml
  label: DNS Doctor Domains API
  slug: dnsdoctor-dev-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsdoctor-dev/openapi/dnsdoctor-dev-domains-api-openapi.yml
- filename: dnsdoctor-dev-monitoring-api-openapi.yml
  format: yaml
  label: DNS Doctor Monitoring API
  slug: dnsdoctor-dev-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsdoctor-dev/openapi/dnsdoctor-dev-monitoring-api-openapi.yml
- filename: dnsdoctor-dev-scan-api-openapi.yml
  format: yaml
  label: DNS Doctor Scan API
  slug: dnsdoctor-dev-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsdoctor-dev/openapi/dnsdoctor-dev-scan-api-openapi.yml
- filename: dnsdoctor-dev-tools-api-openapi.yml
  format: yaml
  label: DNS Doctor Tools API
  slug: dnsdoctor-dev-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsdoctor-dev/openapi/dnsdoctor-dev-tools-api-openapi.yml
- filename: dnsdoctor-dev-watch-api-openapi.yml
  format: yaml
  label: DNS Doctor Watch API
  slug: dnsdoctor-dev-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsdoctor-dev/openapi/dnsdoctor-dev-watch-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dnsdoctor.dev
  spf: true
hosts:
- cert_expires: Jan 26 18:23:32 2027 GMT
  host: dnsdoctor.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DNS Doctor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DNS Doctor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DNS Doctor
provider_slug: dnsdoctor-dev
slug: dnsdoctor-dev-domain-security
source_filename: dnsdoctor-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dnsdoctor.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 18:23:32 2027 GMT\n  hsts: false\ndomains:\n- domain: dnsdoctor.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dnsdoctor-dev/security/dnsdoctor-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- DNS
- DNS Tools
- Email Authentication
- Web Application
---
