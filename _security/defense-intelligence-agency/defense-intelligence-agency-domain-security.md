---
description: ''
domains:
- caa:
  - 128 issue "digicert.com"
  - 128 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dia.mil
  spf: true
hosts:
- cert_expires: Aug 17 15:25:38 2026 GMT
  host: www.dia.mil
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Defense Intelligence Agency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defense Intelligence Agency, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Defense Intelligence Agency
provider_slug: defense-intelligence-agency
slug: defense-intelligence-agency-domain-security
source_filename: defense-intelligence-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dia.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 15:25:38 2026 GMT\n  hsts: null\ndomains:\n- domain: dia.mil\n  dnssec: true\n  caa:\n  - 128 issue \"digicert.com\"\n  - 128 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defense-intelligence-agency/refs/heads/main/security/defense-intelligence-agency-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Defense
- Department of Defense
- DIA
- Federal Government
- Intelligence
- Military Intelligence
- National Security
---
