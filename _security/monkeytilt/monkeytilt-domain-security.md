---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: monkeytilt.com
  spf: true
hosts:
- cert_expires: Oct 11 06:33:02 2026 GMT
  host: monkeytilt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Monkeytilt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MonkeyTilt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: MonkeyTilt
provider_slug: monkeytilt
slug: monkeytilt-domain-security
source_filename: monkeytilt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monkeytilt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 06:33:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: monkeytilt.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monkeytilt/refs/heads/main/security/monkeytilt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Casino
- Sportsbook
- iGaming
- Gambling
- Betting
---
