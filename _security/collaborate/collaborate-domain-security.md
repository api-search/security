---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: collaborate.com
  mx: []
  nameservers:
  - ns1.markmonitor.com
  - ns2.markmonitor.com
  - ns3.markmonitor.com
  - ns4.markmonitor.com
  - ns5.markmonitor.com
  - ns6.markmonitor.com
  - ns7.markmonitor.com
  spf: false
hosts:
- host: collaborate.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http: true
  http_status: 301
  https: false
  https_error: connection timed out (15s)
  redirects_to: https://www.webex.com/
  security_headers:
  - x-content-type-options: nosniff
  - x-frame-options: DENY
  - referrer-policy: no-referrer
  - content-security-policy: default-src 'none'
kind: domain-security
layout: security
method: probed
name: Collaborate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Collaborate *, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Collaborate *
provider_slug: collaborate
slug: collaborate-domain-security
source_filename: collaborate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live probe of collaborate.com (curl HEAD + dig)\nnotes: >-\n  collaborate.com no longer hosts a product. Plain HTTP returns 301 to\n  https://www.webex.com/ (Cisco Webex); HTTPS on the apex times out and serves\n  no site of its own. Nameservers are MarkMonitor, consistent with a\n  brand-protection / redirect domain held by the acquirer rather than an\n  operating company. Absence of records below is recorded fact, not a gap in\n  the probe.\nhosts:\n- host: collaborate.com\n  https: false\n  https_error: connection timed out (15s)\n  http: true\n  http_status: 301\n  redirects_to: https://www.webex.com/\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  security_headers:\n  - x-content-type-options: nosniff\n  - x-frame-options: DENY\n  - referrer-policy: no-referrer\n  - content-security-policy: \"default-src 'none'\"\ndomains:\n- domain: collaborate.com\n  dnssec: false\n  caa: []\n  spf: false\n\
  \  dmarc: false\n  dmarc_policy: null\n  mx: []\n  nameservers:\n  - ns1.markmonitor.com\n  - ns2.markmonitor.com\n  - ns3.markmonitor.com\n  - ns4.markmonitor.com\n  - ns5.markmonitor.com\n  - ns6.markmonitor.com\n  - ns7.markmonitor.com\nwell_known_probe:\n- path: /.well-known/security.txt\n  status: null\n  result: connection failed (no HTTPS listener)\n- path: /.well-known/openid-configuration\n  status: null\n  result: connection failed (no HTTPS listener)\n- path: /.well-known/oauth-authorization-server\n  status: null\n  result: connection failed (no HTTPS listener)\n- path: /.well-known/api-catalog\n  status: null\n  result: connection failed (no HTTPS listener)\n- path: /.well-known/ai-plugin.json\n  status: null\n  result: connection failed (no HTTPS listener)\n- path: /llms.txt\n  status: null\n  result: connection failed (no HTTPS listener)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collaborate/refs/heads/main/security/collaborate-domain-security.yml
summary_line: HSTS
tags:
- Company
- Enterprise
- Collaboration
- Team Messaging
- File Sharing
- Task Management
- Mobile
- Acquired
---
