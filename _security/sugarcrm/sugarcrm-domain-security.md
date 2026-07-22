---
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sugarcrm.com
  spf: true
hosts:
- cert_expires: Oct  3 23:26:18 2026 GMT
  host: www.sugarcrm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sugarcrm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SugarCRM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SugarCRM
provider_slug: sugarcrm
slug: sugarcrm-domain-security
source_filename: sugarcrm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sugarcrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:26:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sugarcrm.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sugarcrm/refs/heads/main/security/sugarcrm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Saas
- CRM
- Sales
- Marketing
- Customer Service
- Sales Automation
- REST API
---
