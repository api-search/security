---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getreliancehealth.com
  spf: true
hosts:
- cert_expires: Aug 22 02:43:06 2026 GMT
  host: www.getreliancehealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reliance Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reliance Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reliance Health
provider_slug: reliance-health
slug: reliance-health-domain-security
source_filename: reliance-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getreliancehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 02:43:06 2026 GMT\n  hsts: false\ndomains:\n- domain: getreliancehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reliance-health/refs/heads/main/security/reliance-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Health Insurance
- HMO
- Telemedicine
- Employee Benefits
- Insurtech
- Africa
- Nigeria
---
