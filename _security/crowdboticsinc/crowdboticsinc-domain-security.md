---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crowdbotics.com
  spf: true
hosts:
- cert_expires: Jan  5 08:43:27 2027 GMT
  host: crowdbotics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crowdboticsinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crowdboticsinc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crowdboticsinc
provider_slug: crowdboticsinc
slug: crowdboticsinc-domain-security
source_filename: crowdboticsinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crowdbotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 08:43:27 2027 GMT\n  hsts: false\ndomains:\n- domain: crowdbotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdboticsinc/refs/heads/main/security/crowdboticsinc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Software Development
- Platform
- Automation
---
