---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: alcometer.de
  spf: true
hosts:
- cert_expires: Dec  2 00:08:53 2026 GMT
  host: alcometer.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alcometer De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Webersheim, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Webersheim
provider_slug: alcometer-de
slug: alcometer-de-domain-security
source_filename: alcometer-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alcometer.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 00:08:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alcometer.de\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/alcometer-de/security/alcometer-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Alcohol
- Health
- Calculator
- Germany
- MCP
---
