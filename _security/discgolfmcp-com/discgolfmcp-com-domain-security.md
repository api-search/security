---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: discgolfmcp.com
  spf: false
hosts:
- cert_expires: Jan 16 18:58:34 2027 GMT
  host: discgolfmcp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Discgolfmcp Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Disc Golf MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Disc Golf MCP
provider_slug: discgolfmcp-com
slug: discgolfmcp-com-domain-security
source_filename: discgolfmcp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: discgolfmcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 18:58:34 2027 GMT\n  hsts: false\ndomains:\n- domain: discgolfmcp.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/discgolfmcp-com/security/discgolfmcp-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Disc Golf
- Sports
- Data
- PDGA
---
