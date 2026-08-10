---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aibank.com
  spf: true
- domain: citicaibank.cn
  note: Alternate portal domain (www.citicaibank.cn) discovered from links on the aibank.com homepage; not separately DNS-profiled this round.
hosts:
- cert_expires: null
  host: www.aibank.com
  hsts: null
  https: true
  https_observed: '2026-08-06'
  note: HTTPS 200 confirmed by direct fetch; TLS version, certificate expiry and HSTS were not captured before the origin began timing out this source IP. Re-probe next round.
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Ai Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Bank, probed live across 1 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AI Bank
provider_slug: ai-bank
slug: ai-bank-domain-security
source_filename: ai-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts\n\n# NOTE ON THE HTTP RESULT. www.aibank.com served HTTPS 200 to this run earlier in the\n# same pass (the homepage HTML was retrieved over TLS and parsed). Partway through\n# contract discovery the origin began refusing our source IP — every subsequent request\n# to www.aibank.com, www.citicaibank.cn and their sub-paths returned curl exit 28\n# (connection timed out) rather than a status code. The automated re-probe therefore\n# recorded `https: false`, which is an artifact of that block, not a property of the\n# host. It is corrected below to what was actually observed, with the unobserved TLS\n# fields left null rather than guessed.\nhosts:\n- host: www.aibank.com\n  https: true\n  https_observed: '2026-08-06'\n  tls_version: null\n  cert_expires: null\n  hsts: null\n  note: >-\n    HTTPS 200 confirmed by direct fetch; TLS version, certificate expiry and HSTS were\n    not captured\
  \ before the origin began timing out this source IP. Re-probe next round.\ndomains:\n- domain: aibank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: citicaibank.cn\n  note: >-\n    Alternate portal domain (www.citicaibank.cn) discovered from links on the aibank.com\n    homepage; not separately DNS-profiled this round.\nfindings:\n- No DMARC record on aibank.com — a licensed bank's primary domain with SPF but no DMARC\n  policy, so there is no published handling instruction for spoofed mail.\n- No CAA records — any public CA may issue for aibank.com.\n- No DNSSEC.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai-bank/refs/heads/main/security/ai-bank-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Banking
- Digital Banking
- Financial Services
- Consumer Finance
- SME Lending
- Wealth Management
- FinTech
- China
---
