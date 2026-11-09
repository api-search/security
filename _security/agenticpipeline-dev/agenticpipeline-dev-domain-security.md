---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agenticpipeline.dev
  spf: true
hosts:
- cert_expires: Jan 15 23:44:43 2027 GMT
  host: agenticpipeline.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agenticpipeline Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agentic Pipeline, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agentic Pipeline
provider_slug: agenticpipeline-dev
slug: agenticpipeline-dev-domain-security
source_filename: agenticpipeline-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agenticpipeline.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:44:43 2027 GMT\n  hsts: false\ndomains:\n- domain: agenticpipeline.dev\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/agenticpipeline-dev/security/agenticpipeline-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CI/CD
- DevOps
- Automation
- AI Agents
- GitHub Actions Alternative
- MCP
---
