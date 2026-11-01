---
api_specs:
- filename: uptime-kuma-openapi-generated.yml
  format: yaml
  label: Uptime Kuma API
  slug: uptime-kuma-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptime-kuma/openapi/_ae-authored/uptime-kuma-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kuma.pet
  spf: true
hosts:
- cert_expires: Dec  9 10:54:54 2026 GMT
  host: uptime.kuma.pet
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Uptime Kuma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uptime Kuma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Uptime Kuma
provider_slug: uptime-kuma
slug: uptime-kuma-domain-security
source_filename: uptime-kuma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uptime.kuma.pet\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 10:54:54 2026 GMT\n  hsts: false\ndomains:\n- domain: kuma.pet\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/uptime-kuma/security/uptime-kuma-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Monitoring
- Self-Hosted
- Open-Source
- Dashboard
- Alerts
---
