---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: joingroups.com
  spf: true
hosts:
- cert_expires: Sep 23 23:02:17 2026 GMT
  host: www.joingroups.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Groups Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Groups, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Groups
provider_slug: groups
slug: groups-domain-security
source_filename: groups-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joingroups.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:02:17 2026 GMT\n  hsts: false\ndomains:\n- domain: joingroups.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groups/refs/heads/main/security/groups-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Addiction Treatment
- Opioid Use Disorder
- Medication-Assisted Treatment
- Telehealth
- Behavioral Health
- Recovery
---
