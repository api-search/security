---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nectarsocial.com
  spf: true
hosts:
- cert_expires: Oct 17 11:29:41 2026 GMT
  host: www.nectarsocial.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 00:40:12 2026 GMT
  host: docs.nectarsocial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: mcp.nectarsocial.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nectar Social Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nectar Social, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Nectar Social
provider_slug: nectar-social
slug: nectar-social-domain-security
source_filename: nectar-social-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nectarsocial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 11:29:41 2026 GMT\n  hsts: false\n- host: docs.nectarsocial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:40:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.nectarsocial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nectarsocial.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nectar-social/refs/heads/main/security/nectar-social-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Social-Media
- Community Management
- Social Listening
- Influencer Marketing
- Customer Engagement
- Social Commerce
- MCP
- Agents
- Authentication
---
