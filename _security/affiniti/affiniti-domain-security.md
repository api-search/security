---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: extu.com
  spf: true
hosts:
- cert_expires: Nov 20 09:18:48 2026 GMT
  host: extu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Affiniti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Affiniti, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Affiniti
provider_slug: affiniti
slug: affiniti-domain-security
source_filename: affiniti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: extu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 09:18:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: extu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affiniti/refs/heads/main/security/affiniti-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Channel Marketing
- Marketing Automation
- Through-Channel Marketing
- Partner Marketing
- Incentives
- Loyalty
- Rebates
- Rewards
- B2B SaaS
---
