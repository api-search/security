---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: metlo.com
  spf: true
hosts:
- cert_expires: Jan 14 08:45:43 2027 GMT
  host: metlo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 02:30:29 2026 GMT
  host: docs.metlo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Metlo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metlo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Metlo
provider_slug: metlo
slug: metlo-domain-security
source_filename: metlo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metlo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 08:45:43 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.metlo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 02:30:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: metlo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/metlo/security/metlo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Security
- Cloud-Native
- Real-Time Monitoring
- OpenAPI
- CI/CD Integration
---
