---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: castrolabs.co
  spf: true
hosts:
- cert_expires: Jan  7 07:34:43 2027 GMT
  host: www.castrolabs.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Castro Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Castro Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Castro Labs
provider_slug: castro-labs
slug: castro-labs-domain-security
source_filename: castro-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.castrolabs.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 07:34:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: castrolabs.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/castro-labs/refs/heads/main/security/castro-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Social
- Community
- SaaS
- LGBTQ+
- SanFrancisco
---
