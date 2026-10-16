---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: care-harmony.com
  spf: true
hosts:
- cert_expires: Dec  1 07:14:25 2026 GMT
  host: care-harmony.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Careharmony Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Careharmony, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Careharmony
provider_slug: careharmony
slug: careharmony-domain-security
source_filename: careharmony-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: care-harmony.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 07:14:25 2026 GMT\n  hsts: false\ndomains:\n- domain: care-harmony.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/careharmony/refs/heads/main/security/careharmony-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- ChronicCare
- RemoteMonitoring
- ValueBased
- SaaS
---
