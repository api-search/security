---
description: Domain security posture probed for the Limit Break corporate site and the Apptokens documentation host. Absence of a record is recorded as observed data, not as an error.
domains: []
hosts:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@limitbreak.com"
  - 0 issue "amazon.com"
  - 0 issue "cloudflare.com"
  - 0 issue "digitrust.com"
  cert_expires: Feb 16 17:22:00 2027 GMT
  cert_issuer: GoDaddy.com, Inc.
  dmarc:
  - '"v=DMARC1; p=reject; pct=100; rua=mailto:dmarc-reports-limitbreak@limitbreak.com"'
  dnssec: true
  host: limitbreak.com
  hsts: true
  hsts_header: max-age=31536000; includeSubDomains; preload
  http_status: 403
  https: true
  spf:
  - '"v=spf1 include:secureserver.net include:_spf.google.com ~all"'
  tls_version: TLSv1.3
- caa:
  - 0 issue "amazon.com"
  - 0 issue "cloudflare.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com amazontrust.com awstrust.com amazonaws.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "cloudflare.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@limitbreak.com"
  cert_expires: Sep 17 02:22:08 2026 GMT
  cert_issuer: Google Trust Services
  dmarc:
  - '"v=DMARC1; p=reject; pct=100; rua=mailto:dmarc-reports-apptokens@limitbreak.com"'
  dnssec: false
  host: apptokens.com
  hsts: true
  hsts_header: max-age=31536000; includeSubDomains; preload
  http_status: 200
  https: true
  spf:
  - '"v=spf1 -all"'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Limit Break Domain Security
name_suffix: Domain Security
overview: Domain security posture for Limit Break, probed live across 2 host(s) and 0 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS.
provider_name: Limit Break
provider_slug: limit-break
slug: limit-break-domain-security
source_filename: limit-break-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live TLS/HTTP/DNS probe\ndescription: Domain security posture probed for the Limit Break corporate site and the Apptokens documentation host.\n  Absence of a record is recorded as observed data, not as an error.\nhosts:\n- host: limitbreak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 17:22:00 2027 GMT\n  cert_issuer: GoDaddy.com, Inc.\n  http_status: 403\n  hsts: true\n  hsts_header: max-age=31536000; includeSubDomains; preload\n  dnssec: true\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@limitbreak.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"digitrust.com\"\n  spf:\n  - '\"v=spf1 include:secureserver.net include:_spf.google.com ~all\"'\n  dmarc:\n  - '\"v=DMARC1; p=reject; pct=100; rua=mailto:dmarc-reports-limitbreak@limitbreak.com\"'\n- host: apptokens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires:\
  \ Sep 17 02:22:08 2026 GMT\n  cert_issuer: Google Trust Services\n  http_status: 200\n  hsts: true\n  hsts_header: max-age=31536000; includeSubDomains; preload\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com amazontrust.com awstrust.com amazonaws.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"cloudflare.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@limitbreak.com\"\n  spf:\n  - '\"v=spf1 -all\"'\n  dmarc:\n  -\
  \ '\"v=DMARC1; p=reject; pct=100; rua=mailto:dmarc-reports-apptokens@limitbreak.com\"'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/limit-break/refs/heads/main/security/limit-break-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Gaming
- Blockchain
- Smart Contracts
- Ethereum
- EVM
- Tokens
- NFT
- DeFi
- Creator Economy
- Solidity
- Agent Skills
---
