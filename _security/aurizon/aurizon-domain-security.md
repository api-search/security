---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:certificate_management@equatetechnologies.com.au"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aurizon.com.au
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: aurizon.com.au
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aurizon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aurizon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aurizon
provider_slug: aurizon
slug: aurizon-domain-security
source_filename: aurizon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aurizon.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: aurizon.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:certificate_management@equatetechnologies.com.au\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aurizon/refs/heads/main/security/aurizon-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Rail Freight
- Logistics
- Transportation
- Mining
- Australia
- Supply Chain
---
