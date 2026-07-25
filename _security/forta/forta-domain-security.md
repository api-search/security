---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: forta.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: forta.network
  spf: true
hosts:
- cert_expires: Sep 29 07:27:09 2026 GMT
  host: forta.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 16:46:58 2026 GMT
  host: docs.forta.network
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 14:31:20 2026 GMT
  host: api.forta.network
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forta, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Forta
provider_slug: forta
slug: forta-domain-security
source_filename: forta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forta.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 07:27:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.forta.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:46:58 2026 GMT\n  hsts: false\n- host: api.forta.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 14:31:20 2026 GMT\n  hsts: null\ndomains:\n- domain: forta.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: forta.network\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forta/refs/heads/main/security/forta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Blockchain
- Web3
- Monitoring
- Threat Detection
- DeFi
- GraphQL
- Alerts
- Smart Contracts
---
