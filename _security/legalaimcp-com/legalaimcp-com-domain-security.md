---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: legalaimcp.com
  spf: false
hosts:
- cert_expires: Jan 11 14:24:18 2027 GMT
  host: legalaimcp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LegalAIMCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LegalAIMCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LegalAIMCP
provider_slug: legalaimcp-com
slug: legalaimcp-com-domain-security
source_filename: legalaimcp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: legalaimcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 14:24:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: legalaimcp.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/legalaimcp-com/security/legalaimcp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Legal Tech
- Artificial Intelligence
- Directory
- MCP
- Law Firms
---
