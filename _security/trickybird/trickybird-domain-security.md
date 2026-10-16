---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; np=reject; rua=mailto:dmarc@trickybird.com; fo=1
  dmarc_subdomain_policy: reject
  dnssec: false
  domain: trickybird.com
  spf: true
  x-reprobed: 2026-10-05 (dig TXT _dmarc.trickybird.com; provider request api-evangelist/trickybird#1)
hosts:
- cert_expires: Dec  8 12:25:59 2026 GMT
  host: trickybird.com
  hsts: true
  hsts_header: max-age=31536000; includeSubDomains; preload
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trickybird Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrickyBird, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TrickyBird
provider_slug: trickybird
slug: trickybird-domain-security
source_filename: trickybird-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trickybird.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 12:25:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  hsts_header: max-age=31536000; includeSubDomains; preload\ndomains:\n- domain: trickybird.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_subdomain_policy: reject\n  dmarc_record: v=DMARC1; p=quarantine; np=reject; rua=mailto:dmarc@trickybird.com; fo=1\n  x-reprobed: '2026-10-05 (dig TXT _dmarc.trickybird.com; provider request api-evangelist/trickybird#1)'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trickybird/refs/heads/main/security/trickybird-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- web proxy
- unblock
- no account
- no install
- Browser
- Agent-Native
- WebMCP
- llms-txt
- Privacy
- network filtering circumvention
---
