---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nsa.gov
  spf: true
hosts:
- cert_expires: Jul 29 18:07:45 2026 GMT
  host: www.nsa.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Security Agency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Security Agency, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Security Agency
provider_slug: national-security-agency
slug: national-security-agency-domain-security
source_filename: national-security-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nsa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 18:07:45 2026 GMT\n  hsts: null\ndomains:\n- domain: nsa.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-security-agency/refs/heads/main/security/national-security-agency-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Intelligence
- Security
---
