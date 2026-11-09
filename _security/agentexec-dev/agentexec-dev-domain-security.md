---
description: ''
domains:
- caa:
  - agentexec-website.onrender.com.
  - gcp-us-west1-1.origin.onrender.com.
  - gcp-us-west1-1.origin.onrender.com.cdn.cloudflare.net.
  dmarc: false
  dnssec: true
  domain: agentexec.dev
  spf: true
hosts:
- cert_expires: Jan 31 15:58:28 2027 GMT
  host: agentexec.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 20:05:10 2027 GMT
  host: api.agentexec.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Agentexec Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentExec, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: AgentExec
provider_slug: agentexec-dev
slug: agentexec-dev-domain-security
source_filename: agentexec-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentexec.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 15:58:28 2027 GMT\n  hsts: false\n- host: api.agentexec.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 20:05:10 2027 GMT\n  hsts: null\ndomains:\n- domain: agentexec.dev\n  dnssec: true\n  caa:\n  - agentexec-website.onrender.com.\n  - gcp-us-west1-1.origin.onrender.com.\n  - gcp-us-west1-1.origin.onrender.com.cdn.cloudflare.net.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentexec-dev/security/agentexec-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Artificial Intelligence
- Automation
- Blockchain
- WebMCP
- Base
- Finance
---
