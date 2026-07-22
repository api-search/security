---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@pointfive.co"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pointfive.co
  spf: true
hosts:
- cert_expires: Sep  6 14:01:41 2026 GMT
  host: www.pointfive.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pointfive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pointfive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Pointfive
provider_slug: pointfive
slug: pointfive-domain-security
source_filename: pointfive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pointfive.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 14:01:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pointfive.co\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@pointfive.co\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pointfive/refs/heads/main/security/pointfive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cloud Saas
- FinOps
- Cloud Cost Optimization
- Cloud Infrastructure
- Kubernetes
- AI Infrastructure
- MCP
---
