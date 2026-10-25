---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: crowdstrike.com
  spf: true
hosts:
- cert_expires: Dec 20 18:08:03 2026 GMT
  host: www.crowdstrike.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 18:21:17 2026 GMT
  host: developer.crowdstrike.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  7 23:59:59 2027 GMT
  host: api.crowdstrike.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Crowdstrike Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CrowdStrike, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CrowdStrike
provider_slug: crowdstrike
slug: crowdstrike-domain-security
source_filename: crowdstrike-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crowdstrike.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 18:08:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.crowdstrike.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 18:21:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.crowdstrike.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: crowdstrike.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdstrike/refs/heads/main/security/crowdstrike-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cybersecurity
- Endpoint Security
- Endpoint Detection and Response
- Threat Intelligence
- Cloud Security
- Identity Protection
- Vulnerability Management
- SIEM
- Security Operations
- MCP
---
