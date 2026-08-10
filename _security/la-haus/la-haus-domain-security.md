---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; pct=100; rua=mailto:postmaster@lahaus.com
  dnssec: false
  domain: lahaus.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:_spf.salesforce.com include:_spf.embluemail.com include:spf.protection.outlook.com include:21568098.spf05.hubspotemail.net ~all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; pct=100; rua=mailto:postmaster@lahaus.com ruf=mailto:postmaster@lahaus.com
  dnssec: false
  domain: lahaus.mx
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:_spf.salesforce.com include:_spf.embluemail.com include:spf.protection.outlook.com ~all
hosts:
- cert_expires: Oct  3 14:01:06 2026 GMT
  host: www.lahaus.com
  hsts: false
  hsts_header: max-age=0
  http_status: 200
  https: true
  note: A Strict-Transport-Security header is sent but with max-age=0, which explicitly clears/disables HSTS rather than enforcing it.
  tls_version: TLSv1.3
- cert_expires: Oct 20 03:58:48 2026 GMT
  host: www.lahaus.mx
  hsts: false
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: api.lahaus.com
  hsts: false
  http_status: 403
  https: true
  note: Private AWS API Gateway. Every anonymous path returns 403 MissingAuthenticationToken.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: La Haus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for La Haus, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: La Haus
provider_slug: la-haus
slug: la-haus-domain-security
source_filename: la-haus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the lahaus.mx and api.lahaus.com\n  hosts observed during contract discovery\nhosts:\n- host: www.lahaus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:01:06 2026 GMT\n  http_status: 200\n  hsts: false\n  hsts_header: max-age=0\n  note: A Strict-Transport-Security header is sent but with max-age=0, which explicitly\n    clears/disables HSTS rather than enforcing it.\n- host: www.lahaus.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 03:58:48 2026 GMT\n  http_status: 200\n  hsts: false\n- host: api.lahaus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  http_status: 403\n  hsts: false\n  note: Private AWS API Gateway. Every anonymous path returns 403 MissingAuthenticationToken.\ndomains:\n- domain: lahaus.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:_spf.salesforce.com\
  \ include:_spf.embluemail.com\n    include:spf.protection.outlook.com include:21568098.spf05.hubspotemail.net ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: v=DMARC1; p=quarantine; pct=100; rua=mailto:postmaster@lahaus.com\n- domain: lahaus.mx\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:_spf.salesforce.com include:_spf.embluemail.com\n    include:spf.protection.outlook.com ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: 'v=DMARC1; p=quarantine; pct=100; rua=mailto:postmaster@lahaus.com\n    ruf=mailto:postmaster@lahaus.com'\nx-evidence:\n  probed: '2026-08-04'\n  tools: [dig, openssl s_client, curl]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/la-haus/refs/heads/main/security/la-haus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- Proptech
- Marketplace
- Housing
- Mortgages
- Brokerage
- Latin America
- Colombia
- Mexico
---
