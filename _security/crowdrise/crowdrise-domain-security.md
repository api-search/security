---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: crowdrise.com
  spf: false
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: crowdrise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Crowdrise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CrowdRise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CrowdRise
provider_slug: crowdrise
slug: crowdrise-domain-security
source_filename: crowdrise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crowdrise.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crowdrise.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdrise/refs/heads/main/security/crowdrise-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Crowdfunding
- Fundraising
- Nonprofit
- Charity
- Donations
- Payments
- Acquired
---
