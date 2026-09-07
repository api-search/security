---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cubicpv.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 1366tech.com
  mx: 1366tech-com.mail.protection.outlook.com
  note: Mail is still live on Microsoft 365 even though the web presence is not.
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com -all
hosts:
- cert_expires: Oct 31 10:38:26 2026 GMT
  cert_issuer: Let's Encrypt
  cert_valid: true
  host: cubicpv.com
  hsts: false
  https: true
  note: SiteGround robot challenge answers 202 on every path probed.
  tls_version: TLSv1.3
- cert_expires: May  4 21:01:29 2024 GMT
  cert_issuer: Let's Encrypt R3
  cert_subject: CN=*.1366tech.com
  cert_valid: false
  host: 1366tech.com
  hsts: false
  https: false
  note: Certificate expired 2024-05-04 and was never renewed; curl and any browser refuse the connection without -k. The last HTTP 200 capture of this site in the Internet Archive is 2021-08-11, weeks after the CubicPV merger closed.
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: 1366 Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1366 Technologies, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 1366 Technologies
provider_slug: 1366-technologies
slug: 1366-technologies-domain-security
source_filename: 1366-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the company's own legacy domain 1366tech.com\nnote: >-\n  1366 Technologies merged into CubicPV (June 2021); cubicpv.com is the surviving corporate host and\n  is wired as the Website pointer. 1366tech.com is still registered and still resolves, and its\n  Microsoft 365 mail records are live, but its TLS certificate expired 2024-05-04 and has not been\n  renewed, so every browser refuses the connection. Both hosts sit behind a SiteGround robot\n  challenge (HTTP 202, sg-captcha: challenge) that answers every path, so no HTTP body could be\n  read; the TLS and DNS findings below are unaffected by that wall.\nhosts:\n- host: cubicpv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 10:38:26 2026 GMT\n  cert_issuer: \"Let's Encrypt\"\n  cert_valid: true\n  hsts: false\n  note: SiteGround robot challenge answers 202 on every path probed.\n- host: 1366tech.com\n  https:\
  \ false\n  tls_version: TLSv1.3\n  cert_subject: CN=*.1366tech.com\n  cert_issuer: \"Let's Encrypt R3\"\n  cert_expires: May  4 21:01:29 2024 GMT\n  cert_valid: false\n  hsts: false\n  note: >-\n    Certificate expired 2024-05-04 and was never renewed; curl and any browser refuse the\n    connection without -k. The last HTTP 200 capture of this site in the Internet Archive is\n    2021-08-11, weeks after the CubicPV merger closed.\ndomains:\n- domain: cubicpv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: 1366tech.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: \"v=spf1 include:spf.protection.outlook.com -all\"\n  dmarc: true\n  dmarc_policy: quarantine\n  mx: 1366tech-com.mail.protection.outlook.com\n  note: Mail is still live on Microsoft 365 even though the web presence is not.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1366-technologies/refs/heads/main/security/1366-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Solar
- Photovoltaics
- Renewable Energy
- Manufacturing
- Semiconductors
- Materials Science
- Cleantech
---
