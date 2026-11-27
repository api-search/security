---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: codecrafted.co.uk
  spf: false
hosts:
- cert_expires: Jan 10 06:13:48 2027 GMT
  host: codecrafted.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CodeCrafted Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodeCrafted, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: CodeCrafted
provider_slug: codecrafted-co-uk
slug: codecrafted-co-uk-domain-security
source_filename: codecrafted-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codecrafted.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 06:13:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: codecrafted.co.uk\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/codecrafted-co-uk/security/codecrafted-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- MCP
- AI Agents
- Design Systems
- Web Development
- Software Development
- Hosting
- United Kingdom
---
