---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getboomerang.ai
  spf: true
hosts:
- cert_expires: Nov 21 07:55:35 2026 GMT
  host: www.getboomerang.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boomerangai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BoomerangAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BoomerangAI
provider_slug: boomerangai
slug: boomerangai-domain-security
source_filename: boomerangai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getboomerang.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 07:55:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getboomerang.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boomerangai/refs/heads/main/security/boomerangai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Sales
- B2B
- Referrals
- Automation
---
