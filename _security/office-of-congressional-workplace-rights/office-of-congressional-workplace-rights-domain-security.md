---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ocwr.gov
  spf: true
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: www.ocwr.gov
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Office Of Congressional Workplace Rights Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Office of Congressional Workplace Rights, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Office of Congressional Workplace Rights
provider_slug: office-of-congressional-workplace-rights
slug: office-of-congressional-workplace-rights-domain-security
source_filename: office-of-congressional-workplace-rights-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ocwr.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ocwr.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/office-of-congressional-workplace-rights/refs/heads/main/security/office-of-congressional-workplace-rights-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
---
