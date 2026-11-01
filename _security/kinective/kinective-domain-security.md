---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kinective.io
  spf: true
hosts:
- cert_expires: Dec 16 10:49:42 2026 GMT
  host: kinective.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kinective Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kinective, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kinective
provider_slug: kinective
slug: kinective-domain-security
source_filename: kinective-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kinective.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 10:49:42 2026 GMT\n  hsts: false\ndomains:\n- domain: kinective.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/kinective/security/kinective-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Banking
- Fintech
- IntelligentBanking
---
