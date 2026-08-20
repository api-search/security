---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: joincrowdhealth.com
  spf: true
hosts:
- cert_expires: Nov  9 07:41:50 2026 GMT
  host: www.joincrowdhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crowdhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CrowdHealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CrowdHealth
provider_slug: crowdhealth
slug: crowdhealth-domain-security
source_filename: crowdhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joincrowdhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 07:41:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: joincrowdhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdhealth/refs/heads/main/security/crowdhealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Health Insurance
- Health Sharing
- Crowdfunding
- Medical Billing
- Consumer Health
- Insurance Alternative
- Fintech
---
