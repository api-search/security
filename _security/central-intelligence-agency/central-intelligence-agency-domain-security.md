---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:caanotices@uce.cia.gov"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cia.gov
  spf: true
hosts:
- cert_expires: Aug 12 23:59:59 2026 GMT
  host: www.cia.gov
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Central Intelligence Agency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Central Intelligence Agency, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Central Intelligence Agency
provider_slug: central-intelligence-agency
slug: central-intelligence-agency-domain-security
source_filename: central-intelligence-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cia.gov\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:caanotices@uce.cia.gov\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/central-intelligence-agency/refs/heads/main/security/central-intelligence-agency-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- FOIA
- Government
- Intelligence
- National Security
- Open Data
- World Factbook
---
