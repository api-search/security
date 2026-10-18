---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crossover.com
  spf: true
hosts:
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: www.crossover.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crossover Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crossover, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crossover
provider_slug: crossover
slug: crossover-domain-security
source_filename: crossover-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crossover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: crossover.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossover/refs/heads/main/security/crossover-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Recruiting
- Remote Work
- Artificial Intelligence
- TalentMarketplace
---
