---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: coremedicalgroup.com
  spf: true
hosts:
- cert_expires: Nov 17 22:49:46 2026 GMT
  host: www.coremedicalgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coremedical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coremedical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Coremedical
provider_slug: coremedical
slug: coremedical-domain-security
source_filename: coremedical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coremedicalgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 22:49:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coremedicalgroup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coremedical/refs/heads/main/security/coremedical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Staffing
- Healthcare
- TravelNursing
- WorkforceSolutions
---
