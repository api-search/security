---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blackbird.ai
  spf: true
hosts:
- cert_expires: Nov 12 16:02:45 2026 GMT
  host: blackbird.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blackbirdai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blackbird.AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blackbird.AI
provider_slug: blackbirdai
slug: blackbirdai-domain-security
source_filename: blackbirdai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blackbird.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 16:02:45 2026 GMT\n  hsts: false\ndomains:\n- domain: blackbird.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackbirdai/refs/heads/main/security/blackbirdai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Risk Intelligence
- Data Analytics
- Enterprise
---
