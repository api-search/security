---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: creatorstack.com
  spf: true
hosts:
- host: www.creatorstack.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.creator'
kind: domain-security
layout: security
method: probed
name: Creator Stack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Creator Stack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Creator Stack
provider_slug: creator-stack
slug: creator-stack-domain-security
source_filename: creator-stack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.creatorstack.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.creator'\n  hsts: null\ndomains:\n- domain: creatorstack.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creator-stack/refs/heads/main/security/creator-stack-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Consumer
- Creator Economy
- Creators
- Membership
- Fan Engagement
- Community
- Content Monetization
- Royalties
---
