---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: energyvault.com
  spf: true
hosts:
- cert_expires: Sep 14 19:56:10 2026 GMT
  host: www.energyvault.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Energy Vault Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Energy Vault, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Energy Vault
provider_slug: energy-vault
slug: energy-vault-domain-security
source_filename: energy-vault-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.energyvault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:56:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: energyvault.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energy-vault/refs/heads/main/security/energy-vault-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Frontier Tech
- Energy Storage
- Energy Management
- Battery Storage
- Gravity Storage
- Green Hydrogen
- Grid Scale
- Renewable Energy
- VaultOS
---
