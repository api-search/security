---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:mad@infor.com"
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; rua=mailto:l5hgamx6@ag.dmarcian.com
  dnssec: true
  domain: baan.com
  ds_records: 1
  mx:
  - mx1.hc3692-74.iphmx.com
  - mx2.hc3692-74.iphmx.com
  spf: true
  spf_record: v=spf1 exists:%{i}.spf.hc3692-74.iphmx.com include:spf.protection.outlook.com -all
- caa:
  - 0 issue "amazon.com"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:mad@infor.com"
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; rua=mailto:l5hgamx6@ag.dmarcian.com
  dnssec: true
  domain: baan.nl
  ds_records: 1
  mx:
  - mx1.hc3692-74.iphmx.com
  - mx2.hc3692-74.iphmx.com
  spf: true
  spf_record: v=spf1 exists:%{i}.spf.hc3692-74.iphmx.com include:spf.protection.outlook.com -all
hosts:
- host: baan.com
  hsts: false
  http: true
  http_status: 301
  https: false
  https_error: TLS handshake failed on port 443
  redirect_to: https://www.infor.com/product-summary/erp/ln/
- host: www.baan.com
  hsts: false
  http: true
  http_status: 301
  https: false
  https_error: TLS handshake failed on port 443
  redirect_to: https://www.infor.com/product-summary/erp/ln/
kind: domain-security
layout: security
method: probed
name: Baan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baan, probed live across 2 host(s) and 2 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Baan
provider_slug: baan
slug: baan-domain-security
source_filename: baan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS (dig) and TLS/HTTP probes of the legacy Baan domains\nnotes: >-\n  The Baan domains are still actively held and hygienically managed by Infor (DNSSEC signed, CAA\n  pinned, SPF and DMARC p=reject, mail routed through Infor's Cisco IronPort tenant and Microsoft 365),\n  but they serve no HTTPS: port 443 does not complete a TLS handshake on either host. Only plaintext\n  HTTP is answered, and it returns a blanket 301 to the Infor LN product page. Recorded as https:\n  false — this is a parked/redirect estate, not a live API host.\nhosts:\n- host: baan.com\n  https: false\n  https_error: TLS handshake failed on port 443\n  http: true\n  http_status: 301\n  redirect_to: https://www.infor.com/product-summary/erp/ln/\n  hsts: false\n- host: www.baan.com\n  https: false\n  https_error: TLS handshake failed on port 443\n  http: true\n  http_status: 301\n  redirect_to: https://www.infor.com/product-summary/erp/ln/\n  hsts: false\n\
  domains:\n- domain: baan.com\n  dnssec: true\n  ds_records: 1\n  caa:\n  - '0 issue \"amazon.com\"'\n  - '0 issue \"digicert.com; cansignhttpexchanges=yes\"'\n  - '0 issue \"letsencrypt.org\"'\n  - '0 issue \"sectigo.com\"'\n  - '0 issuewild \"amazon.com\"'\n  - '0 issuewild \"digicert.com; cansignhttpexchanges=yes\"'\n  - '0 issuewild \"letsencrypt.org\"'\n  - '0 issuewild \"sectigo.com\"'\n  - '0 iodef \"mailto:mad@infor.com\"'\n  spf: true\n  spf_record: v=spf1 exists:%{i}.spf.hc3692-74.iphmx.com include:spf.protection.outlook.com -all\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: v=DMARC1; p=reject; rua=mailto:l5hgamx6@ag.dmarcian.com\n  mx:\n  - mx1.hc3692-74.iphmx.com\n  - mx2.hc3692-74.iphmx.com\n- domain: baan.nl\n  dnssec: true\n  ds_records: 1\n  caa:\n  - '0 issue \"amazon.com\"'\n  - '0 issuewild \"amazon.com\"'\n  - '0 iodef \"mailto:mad@infor.com\"'\n  spf: true\n  spf_record: v=spf1 exists:%{i}.spf.hc3692-74.iphmx.com include:spf.protection.outlook.com -all\n \
  \ dmarc: true\n  dmarc_policy: reject\n  dmarc_record: v=DMARC1; p=reject; rua=mailto:l5hgamx6@ag.dmarcian.com\n  mx:\n  - mx1.hc3692-74.iphmx.com\n  - mx2.hc3692-74.iphmx.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baan/refs/heads/main/security/baan-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Enterprise Resource Planning
- ERP
- Enterprise Software
- Manufacturing
- Supply Chain
- Netherlands
- Acquired
- Legacy
---
