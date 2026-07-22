---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: theleague.com
  spf: true
hosts:
- cert_expires: Sep  3 00:42:49 2026 GMT
  host: www.theleague.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The League Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The League, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The League
provider_slug: the-league
slug: the-league-domain-security
source_filename: the-league-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.theleague.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 00:42:49 2026 GMT\n  hsts: false\ndomains:\n- domain: theleague.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-league/refs/heads/main/security/the-league-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Dating
- Social
- Mobile Application
- Match Group
- Cowboy Ventures
---
