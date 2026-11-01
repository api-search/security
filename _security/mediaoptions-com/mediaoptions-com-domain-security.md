---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mediaoptions.com
  spf: true
hosts:
- cert_expires: Dec 14 18:32:17 2026 GMT
  host: mediaoptions.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mediaoptions Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Humu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Humu
provider_slug: mediaoptions-com
slug: mediaoptions-com-domain-security
source_filename: mediaoptions-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mediaoptions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 18:32:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mediaoptions.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mediaoptions-com/security/mediaoptions-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
