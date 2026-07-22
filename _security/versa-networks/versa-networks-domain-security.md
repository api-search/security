---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: versa-networks.com
  spf: true
hosts:
- cert_expires: Sep 13 22:40:14 2026 GMT
  host: versa-networks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Versa Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Versa Networks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Versa Networks
provider_slug: versa-networks
slug: versa-networks-domain-security
source_filename: versa-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: versa-networks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 22:40:14 2026 GMT\n  hsts: false\ndomains:\n- domain: versa-networks.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/versa-networks/refs/heads/main/security/versa-networks-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Networking
- Security
- SASE
- SD-WAN
- SSE
- Zero Trust
- ZTNA
- Cybersecurity
- Cloud Networking
- Infrastructure
- MCP
---
