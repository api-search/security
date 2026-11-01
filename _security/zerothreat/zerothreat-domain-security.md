---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: zerothreat.ai
  spf: true
hosts:
- cert_expires: Dec 23 16:25:04 2026 GMT
  host: zerothreat.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zerothreat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZeroThreat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ZeroThreat
provider_slug: zerothreat
slug: zerothreat-domain-security
source_filename: zerothreat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zerothreat.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 16:25:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: zerothreat.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/zerothreat/security/zerothreat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Pentesting
- Web Application Security
- API Security
- DevOps
- Enterprise Security
- Compliance
---
