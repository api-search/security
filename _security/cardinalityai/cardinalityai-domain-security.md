---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cardyai.com
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: www.cardyai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cardinalityai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cardinalityai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cardinalityai
provider_slug: cardinalityai
slug: cardinalityai-domain-security
source_filename: cardinalityai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cardyai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cardyai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardinalityai/refs/heads/main/security/cardinalityai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- SaaS
- Case Management
- Government
---
