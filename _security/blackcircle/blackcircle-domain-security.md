---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: theblackcircle.com
  spf: true
hosts:
- cert_expires: Nov 12 08:15:51 2026 GMT
  host: theblackcircle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blackcircle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blackcircle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Blackcircle
provider_slug: blackcircle
slug: blackcircle-domain-security
source_filename: blackcircle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theblackcircle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 08:15:51 2026 GMT\n  hsts: false\ndomains:\n- domain: theblackcircle.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackcircle/refs/heads/main/security/blackcircle-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Wealth Management
- Private Banking
- Investment
- Multi-jurisdictional
---
