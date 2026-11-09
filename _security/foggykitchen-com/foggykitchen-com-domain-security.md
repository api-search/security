---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: foggykitchen.com
  spf: true
hosts:
- cert_expires: Dec 24 13:32:12 2026 GMT
  host: foggykitchen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Foggykitchen Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FoggyKitchen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FoggyKitchen
provider_slug: foggykitchen-com
slug: foggykitchen-com-domain-security
source_filename: foggykitchen-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foggykitchen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 13:32:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: foggykitchen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/foggykitchen-com/security/foggykitchen-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Education
- Terraform
- Azure
- OCI
---
