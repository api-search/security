---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: obd-vault.com
  spf: true
hosts:
- cert_expires: Jan 31 15:37:52 2027 GMT
  host: obd-vault.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OBD Vault Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OBD Vault, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: OBD Vault
provider_slug: obd-vault-com
slug: obd-vault-com-domain-security
source_filename: obd-vault-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: obd-vault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 15:37:52 2027 GMT\n  hsts: false\ndomains:\n- domain: obd-vault.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/obd-vault-com/security/obd-vault-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Automotive
- Diagnostics
- Mobile App
- OBD-II
---
