---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lseg.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: rua@lseg.com
  dnssec: true
  domain: acadia.inc
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: rua@lseg.com
  dnssec: false
  domain: acadiasoft.com
  note: apex has no A record; only portal.acadiasoft.com still resolves
  spf: true
hosts:
- cert_expires: Apr  6 23:59:59 2027 GMT
  host: www.lseg.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 00:18:58 2026 GMT
  cert_issuer: Google Trust Services WE1
  host: acadia.inc
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: serves HTTP 301 to https://www.lseg.com/en/post-trade/solutions/acadia for every path probed, including all /.well-known/* paths
  tls_version: TLSv1.3
- cert_expires: Apr  6 23:59:59 2027 GMT
  cert_issuer: Sectigo Public Server Authentication CA OV R36
  host: portal.acadiasoft.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Atlassian Confluence customer documentation portal; 302s every anonymous request to an OAuth2 authorization endpoint (realm=docportal)
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Acadiasoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acadia, probed live across 3 host(s) and 3 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Acadia
provider_slug: acadiasoft
slug: acadiasoft-domain-security
source_filename: acadiasoft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the apis.yml Website host plus Acadia's own registrable\n  domains (acadia.inc, acadiasoft.com) and the live customer portal host\nnote: 'Acadia''s own domain acadia.inc still resolves and terminates TLS but serves only\n  a blanket 301 to www.lseg.com; acadiasoft.com no longer resolves at the apex. The\n  DMARC aggregate/forensic mailboxes on BOTH Acadia domains are @lseg.com, which is\n  independent confirmation that LSEG now operates the mail and DNS estate.'\nhosts:\n- host: www.lseg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: acadia.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services WE1\n  cert_expires: Oct 23 00:18:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: serves HTTP 301 to https://www.lseg.com/en/post-trade/solutions/acadia\
  \ for every\n    path probed, including all /.well-known/* paths\n- host: portal.acadiasoft.com\n  https: true\n  tls_version: TLSv1.2\n  cert_issuer: Sectigo Public Server Authentication CA OV R36\n  cert_expires: Apr  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Atlassian Confluence customer documentation portal; 302s every anonymous request\n    to an OAuth2 authorization endpoint (realm=docportal)\ndomains:\n- domain: lseg.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: acadia.inc\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_rua: rua@lseg.com\n- domain: acadiasoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_rua: rua@lseg.com\n  note: apex has no A record; only portal.acadiasoft.com still resolves\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acadiasoft/refs/heads/main/security/acadiasoft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Capital Markets
- Derivatives
- Risk Management
- Collateral Management
- Margin
- Post Trade
- Regulatory Compliance
---
