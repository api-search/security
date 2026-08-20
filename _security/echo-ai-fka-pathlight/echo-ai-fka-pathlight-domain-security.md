---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: echoai.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pathlight.com
  note: NS still delegated to AWS Route 53 and email records retained, but no web A record
  spf: true
hosts:
- cert_expires: Oct 12 12:43:41 2026 GMT
  host: www.echoai.com
  hsts: null
  https: true
  note: TLS terminates, but every path returns HTTP 404 (Framer "Site Not Found")
  tls_version: TLSv1.3
- host: www.pathlight.com
  https: false
  note: legacy brand host; DNS resolution fails (no A record)
kind: domain-security
layout: security
method: probed
name: Echo Ai Fka Pathlight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Echo AI (fka Pathlight), probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Echo AI (fka Pathlight)
provider_slug: echo-ai-fka-pathlight
slug: echo-ai-fka-pathlight-domain-security
source_filename: echo-ai-fka-pathlight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.echoai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 12:43:41 2026 GMT\n  hsts: null\n  note: TLS terminates, but every path returns HTTP 404 (Framer \"Site Not Found\")\n- host: www.pathlight.com\n  https: false\n  note: legacy brand host; DNS resolution fails (no A record)\ndomains:\n- domain: echoai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pathlight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  note: NS still delegated to AWS Route 53 and email records retained, but no web A record\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echo-ai-fka-pathlight/refs/heads/main/security/echo-ai-fka-pathlight-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Conversation Intelligence
- Customer Experience
- Customer-Support
- Artificial Intelligence
- Analytics
---
