---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zibralabs.ai
  mx: google-workspace
  spf: true
  spf_record: v=spf1 include:dc-aa8e722993._spfm.zibralabs.ai ~all
hosts:
- cert_expires: Sep 30 18:51:16 2026 GMT
  cert_issuer: Let's Encrypt
  cert_not_before: Jul  2 18:51:17 2026 GMT
  cert_subject: zibralabs.ai
  host: zibralabs.ai
  hsts: true
  hsts_max_age: 31556952
  https: true
  server: GitHub.com
kind: domain-security
layout: security
method: probed
name: Zibra Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zibra Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zibra Labs
provider_slug: zibra-labs
slug: zibra-labs-domain-security
source_filename: zibra-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the Zibra Labs corporate host (no API base hosts published yet)\nhosts:\n- host: zibralabs.ai\n  https: true\n  server: GitHub.com\n  cert_issuer: Let's Encrypt\n  cert_subject: zibralabs.ai\n  cert_not_before: Jul  2 18:51:17 2026 GMT\n  cert_expires: Sep 30 18:51:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: zibralabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:dc-aa8e722993._spfm.zibralabs.ai ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  mx: google-workspace\nnotes: >-\n  Zibra Labs (YC Spring 2026) currently publishes only a GitHub Pages marketing\n  site at zibralabs.ai; there is no API base host to probe yet. Values above are\n  for the corporate domain. HSTS is present, TLS is a valid Let's Encrypt\n  certificate, SPF and DMARC (p=quarantine) are configured, mail is Google\n  Workspace. No CAA record and no DNSSEC were observed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zibra-labs/refs/heads/main/security/zibra-labs-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Company
- Distributed Compute
- AI Infrastructure
- GPU
- Cloud
- Machine Learning
- Y Combinator
---
