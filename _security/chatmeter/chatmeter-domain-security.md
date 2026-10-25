---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: chatmeter.com
  spf: true
hosts:
- cert_expires: Nov 22 11:02:22 2026 GMT
  host: www.chatmeter.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 02:47:28 2026 GMT
  host: support.chatmeter.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 10:59:01 2026 GMT
  host: live.chatmeter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Chatmeter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chatmeter, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Chatmeter
provider_slug: chatmeter
slug: chatmeter-domain-security
source_filename: chatmeter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chatmeter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 11:02:22 2026 GMT\n  hsts: false\n- host: support.chatmeter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 02:47:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: live.chatmeter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 10:59:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chatmeter.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatmeter/refs/heads/main/security/chatmeter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Reputation Management
- Local SEO
- Listings Management
- Review Management
- Social Media
- Multi-Location
- Competitive Intelligence
---
