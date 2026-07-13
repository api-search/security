---
api_specs:
- filename: unisys-stealth-ecoapi-openapi.yaml
  format: yaml
  label: Unisys Stealth EcoAPI
  slug: unisys-stealth-ecoapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unisys/refs/heads/main/openapi/unisys-stealth-ecoapi-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: unisys.com
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: stealthsecurity.unisys.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unisys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unisys, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Unisys
provider_slug: unisys
slug: unisys-domain-security
source_filename: unisys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stealthsecurity.unisys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: unisys.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unisys/refs/heads/main/security/unisys-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Fortune 1000
- Security
- Zero Trust
- Network Security
- IT Services
- Cybersecurity
- Enterprise Technology
---
