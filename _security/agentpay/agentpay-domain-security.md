---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workers.dev
  spf: true
hosts:
- cert_expires: Dec 30 02:32:36 2026 GMT
  host: agentpay.agentpay-apis.workers.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentPay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AgentPay
provider_slug: agentpay
slug: agentpay-domain-security
source_filename: agentpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentpay.agentpay-apis.workers.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 02:32:36 2026 GMT\n  hsts: false\ndomains:\n- domain: workers.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentpay/refs/heads/main/security/agentpay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API
- AI
- Extraction
- Lookup
- Tools
---
