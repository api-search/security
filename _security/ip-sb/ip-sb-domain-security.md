---
api_specs:
- filename: ip-sb-openapi-generated.yml
  format: yaml
  label: IP.SB API
  slug: ip-sb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ip-sb/openapi/_ae-authored/ip-sb-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ip.sb
  spf: true
hosts:
- cert_expires: Jan  8 04:20:33 2027 GMT
  host: ip.sb
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ip Sb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IP.SB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: IP.SB
provider_slug: ip-sb
slug: ip-sb-domain-security
source_filename: ip-sb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ip.sb\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 04:20:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ip.sb\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ip-sb/security/ip-sb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- API
- IP
- GeoIP
- DNS
---
