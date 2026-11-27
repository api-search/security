---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: filingspy.com
  spf: true
hosts:
- cert_expires: Dec 10 03:05:20 2026 GMT
  host: filingspy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FilingSpy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FilingSpy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FilingSpy
provider_slug: filingspy-com
slug: filingspy-com-domain-security
source_filename: filingspy-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: filingspy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 03:05:20 2026 GMT\n  hsts: false\ndomains:\n- domain: filingspy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/filingspy-com/security/filingspy-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- SEC Filings
- 13F
- Insider Trading
- Investor Tracking
- Financial Data
- MCP
- Agents
- Stock Market
---
