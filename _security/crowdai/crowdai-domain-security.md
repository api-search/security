---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crowdai.com
  spf: true
hosts:
- host: www.crowdai.com
  https: false
kind: domain-security
layout: security
method: probed
name: Crowdai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CrowdAI, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CrowdAI
provider_slug: crowdai
slug: crowdai-domain-security
source_filename: crowdai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crowdai.com\n  https: false\ndomains:\n- domain: crowdai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdai/refs/heads/main/security/crowdai-domain-security.yml
summary_line: DMARC
tags:
- Company
- Ai
---
