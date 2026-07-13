---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nationalguard.mil
  spf: true
hosts:
- cert_expires: Aug 17 15:25:38 2026 GMT
  host: www.nationalguard.mil
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Army National Guard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Army National Guard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Army National Guard
provider_slug: army-national-guard
slug: army-national-guard-domain-security
source_filename: army-national-guard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nationalguard.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 15:25:38 2026 GMT\n  hsts: null\ndomains:\n- domain: nationalguard.mil\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/army-national-guard/refs/heads/main/security/army-national-guard-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Military
- Defense
- National Guard
---
