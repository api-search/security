---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airflows.com
  spf: true
hosts:
- cert_expires: Dec 10 05:55:51 2026 GMT
  host: airflows.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Airflows Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airflows, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Airflows
provider_slug: airflows
slug: airflows-domain-security
source_filename: airflows-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airflows.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 05:55:51 2026 GMT\n  hsts: false\ndomains:\n- domain: airflows.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/airflows/security/airflows-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Enterprise
- SaaS
- Operational-Intelligence
---
