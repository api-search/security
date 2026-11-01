---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tataadvancedsystems.com
  spf: true
hosts:
- cert_expires: Dec 19 04:42:48 2026 GMT
  host: www.tataadvancedsystems.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tata Advanced Systems Limited Tasl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tata Advanced Systems Limited (TASL), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tata Advanced Systems Limited (TASL)
provider_slug: tata-advanced-systems-limited-tasl
slug: tata-advanced-systems-limited-tasl-domain-security
source_filename: tata-advanced-systems-limited-tasl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tataadvancedsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 04:42:48 2026 GMT\n  hsts: false\ndomains:\n- domain: tataadvancedsystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/tata-advanced-systems-limited-tasl/security/tata-advanced-systems-limited-tasl-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Aerospace
- Defence
- Technology
- Manufacturing
- Space
---
