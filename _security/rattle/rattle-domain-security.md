---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: gorattle.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vonlabs.ai
  spf: true
hosts:
- cert_expires: Oct 11 19:51:40 2026 GMT
  host: www.gorattle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:22:18 2026 GMT
  host: vonlabs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: successor brand host (Rattle rebranded its forward product to Von, 2026-05-29)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rattle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rattle, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Rattle
provider_slug: rattle
slug: rattle-domain-security
source_filename: rattle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + the Von (vonlabs.ai) successor domain\nhosts:\n- host: www.gorattle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 19:51:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: vonlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:22:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: successor brand host (Rattle rebranded its forward product to Von, 2026-05-29)\ndomains:\n- domain: gorattle.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: vonlabs.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nnotes: >-\n  gorattle.com is DNSSEC-signed but publishes no CAA record;\
  \ vonlabs.ai publishes a\n  six-issuer CAA set but is not DNSSEC-signed. Both enforce HSTS with a one-year\n  max-age and negotiate TLS 1.3. No security.txt is served on either registrable\n  domain (see well-known/rattle-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rattle/refs/heads/main/security/rattle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Sales
- RevOps
- CRM
- Salesforce
- Slack
- Microsoft Teams
- Sales Automation
- Revenue Intelligence
- Workflow Automation
- Artificial Intelligence
---
