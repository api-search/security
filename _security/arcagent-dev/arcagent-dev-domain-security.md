---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: false
  dnssec: false
  domain: arcagent.dev
  spf: false
hosts:
- cert_expires: Jan 30 02:59:36 2027 GMT
  host: arcagent.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arcagent Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ArcAgent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ArcAgent
provider_slug: arcagent-dev
slug: arcagent-dev-domain-security
source_filename: arcagent-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arcagent.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 02:59:36 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: arcagent.dev\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/arcagent-dev/security/arcagent-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Bounties
- Software Development
- Outsourcing
- Automation
---
