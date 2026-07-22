---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: springlabs.com
  spf: true
hosts:
- cert_expires: Aug 26 10:14:57 2026 GMT
  host: springlabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Springcoin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Springcoin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Springcoin
provider_slug: springcoin
slug: springcoin-domain-security
source_filename: springcoin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: springlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 10:14:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: springlabs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/springcoin/refs/heads/main/security/springcoin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Compliance
- Financial Services
- Customer Experience
- Governance Risk Compliance
- AI Agents
---
