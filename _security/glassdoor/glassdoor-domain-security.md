---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "geotrust.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: glassdoor.com
  spf: true
hosts:
- cert_expires: Sep 26 03:45:16 2026 GMT
  host: www.glassdoor.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 22:04:17 2026 GMT
  host: api.glassdoor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glassdoor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glassdoor, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Glassdoor
provider_slug: glassdoor
slug: glassdoor-domain-security
source_filename: glassdoor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.glassdoor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 03:45:16 2026 GMT\n  hsts: null\n- host: api.glassdoor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 22:04:17 2026 GMT\n  hsts: false\ndomains:\n- domain: glassdoor.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"geotrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glassdoor/refs/heads/main/security/glassdoor-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Employer Reviews
- Job Search
- Salaries
- Recruitment
- Employer Branding
---
