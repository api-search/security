---
description: ''
domains:
- caa:
  - agentaddress.onrender.com.
  - gcp-us-west1-1.origin.onrender.com.
  - gcp-us-west1-1.origin.onrender.com.cdn.cloudflare.net.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: agentaddress.dev
  spf: false
hosts:
- cert_expires: Dec 15 00:18:04 2026 GMT
  host: agentaddress.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentaddress Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentAddress, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: AgentAddress
provider_slug: agentaddress-dev
slug: agentaddress-dev-domain-security
source_filename: agentaddress-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentaddress.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 00:18:04 2026 GMT\n  hsts: false\ndomains:\n- domain: agentaddress.dev\n  dnssec: true\n  caa:\n  - agentaddress.onrender.com.\n  - gcp-us-west1-1.origin.onrender.com.\n  - gcp-us-west1-1.origin.onrender.com.cdn.cloudflare.net.\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agentaddress-dev/security/agentaddress-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Webhook
- Email
- Agents
---
