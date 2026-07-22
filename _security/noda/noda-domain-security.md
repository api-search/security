---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: noda.ai
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: noda.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Noda
provider_slug: noda
slug: noda-domain-security
source_filename: noda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: noda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: noda.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noda/refs/heads/main/security/noda-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Agentic AI
- Building Operations
- Commercial Real Estate
- Energy Management
- Smart Buildings
- PropTech
- Building Automation
- Sustainability
---
