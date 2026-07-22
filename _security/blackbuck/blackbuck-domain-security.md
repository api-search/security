---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:devops.jira@blackbuck.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blackbuck.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.blackbuck.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blackbuck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlackBuck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BlackBuck
provider_slug: blackbuck
slug: blackbuck-domain-security
source_filename: blackbuck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blackbuck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: blackbuck.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:devops.jira@blackbuck.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackbuck/refs/heads/main/security/blackbuck-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplaces
- Logistics
- Trucking
- Transportation
- Fintech
- Supply Chain
- India
---
